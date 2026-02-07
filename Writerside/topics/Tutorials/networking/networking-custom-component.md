# Custom Networked Component

This tutorial walks through building a replicated health component from scratch. You will create a `plNetworkComponent` subclass, use `plNetSerializeAttribute` with replication conditions, and react to state changes on clients.

## Prerequisites

* A working network connection (see [Getting Started](networking-getting-started.md)).
* Familiarity with Plasma's [component system](components.md) and [reflection](reflection-system.md).

## What We Are Building

A `HealthComponent` that:

* Tracks current and max health on the server.
* Replicates health to all clients (for health bars, damage numbers).
* Replicates max health only on initial sync (it does not change often).
* Sends the "is alive" flag to all clients but the shield value only to the owner.

## Step 1: Define the Component

```c++
// HealthComponent.h
#pragma once

#include <NetworkPlugin/Components/NetworkComponent.h>

using HealthComponentManager = plComponentManagerSimple<class HealthComponent, plComponentUpdateType::Always>;

class HealthComponent : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(HealthComponent, plNetworkComponent, HealthComponentManager);

public:
  HealthComponent() = default;
  virtual ~HealthComponent() = default;

  // Public API
  void TakeDamage(float fAmount);
  void Heal(float fAmount);
  bool IsAlive() const { return m_bIsAlive; }
  float GetHealth() const { return m_fCurrentHealth; }
  float GetHealthPercent() const { return m_fMaxHealth > 0 ? m_fCurrentHealth / m_fMaxHealth : 0; }

  // Replicated properties
  float m_fCurrentHealth = 100.0f;
  float m_fMaxHealth = 100.0f;
  float m_fShield = 0.0f;
  bool m_bIsAlive = true;

protected:
  virtual void OnSimulationStarted() override;
  virtual void Update() override;
};
```

## Step 2: Set Up Reflection with Replication Conditions

```c++
// HealthComponent.cpp
#include "HealthComponent.h"
#include <NetworkPlugin/Core/NetworkSerialize.h>

// clang-format off
PL_BEGIN_COMPONENT_TYPE(HealthComponent, 1, plComponentMode::Static)
{
  PL_BEGIN_PROPERTIES
  {
    // Health -- replicated to all clients, only when value changes
    PL_NET_PROPERTY_ON_CHANGE("CurrentHealth", m_fCurrentHealth),

    // Max health -- only sent during initial sync (late-joiner)
    PL_NET_PROPERTY_INITIAL_ONLY("MaxHealth", m_fMaxHealth),

    // Shield -- only sent to the owning client (private info)
    PL_NET_PROPERTY_OWNER_ONLY("Shield", m_fShield),

    // IsAlive -- replicated to all clients, every tick
    PL_NET_PROPERTY("IsAlive", m_bIsAlive),
  }
  PL_END_PROPERTIES;
  PL_BEGIN_ATTRIBUTES
  {
    new plCategoryAttribute("Gameplay"),
  }
  PL_END_ATTRIBUTES;
}
PL_END_COMPONENT_TYPE
// clang-format on
```

### What Each Macro Does

| Macro | Effect |
|-------|--------|
| `PL_NET_PROPERTY_ON_CHANGE` | Only replicates when the value changes from the last sent value. Saves bandwidth when health is not changing. |
| `PL_NET_PROPERTY_INITIAL_ONLY` | Sent once during late-joiner sync. Max health rarely changes, so there is no need to send it every tick. |
| `PL_NET_PROPERTY_OWNER_ONLY` | Shield is private to the owning player. Other clients do not receive this value. |
| `PL_NET_PROPERTY` | Standard replication -- sent to all clients every tick. |

## Step 3: Implement the Logic

```c++
void HealthComponent::OnSimulationStarted()
{
  plNetworkComponent::OnSimulationStarted();

  // Initialize state
  m_fCurrentHealth = m_fMaxHealth;
  m_bIsAlive = true;
}

void HealthComponent::TakeDamage(float fAmount)
{
  if (!m_bIsAlive)
    return;

  // Apply shield first
  if (m_fShield > 0)
  {
    float absorbed = plMath::Min(m_fShield, fAmount);
    m_fShield -= absorbed;
    fAmount -= absorbed;
  }

  m_fCurrentHealth = plMath::Max(0.0f, m_fCurrentHealth - fAmount);

  if (m_fCurrentHealth <= 0)
  {
    m_bIsAlive = false;
  }

  // Mark dirty so the network replicates the new values
  MarkDirty();
}

void HealthComponent::Heal(float fAmount)
{
  if (!m_bIsAlive)
    return;

  m_fCurrentHealth = plMath::Min(m_fMaxHealth, m_fCurrentHealth + fAmount);
  MarkDirty();
}

void HealthComponent::Update()
{
  // Client-side logic (react to replicated state)
  if (!m_pNetworkModule || !m_pNetworkModule->IsClient())
    return;

  // Update health bar UI, play damage effects, etc.
  // m_fCurrentHealth and m_bIsAlive are automatically updated by deserialization
}
```

## Step 4: Use the Component

1. Add `HealthComponent` to your player prefab alongside other network components.
2. On the server, call `TakeDamage()` or `Heal()` when appropriate:

```c++
void ApplyDamageToPlayer(plGameObject* pPlayer, float fDamage)
{
  HealthComponent* pHealth = nullptr;
  if (pPlayer->TryGetComponentOfBaseType(pHealth))
  {
    pHealth->TakeDamage(fDamage);
  }
}
```

3. On clients, read the replicated values to update the UI:

```c++
void UpdateHealthBar(plGameObject* pPlayer)
{
  HealthComponent* pHealth = nullptr;
  if (pPlayer->TryGetComponentOfBaseType(pHealth))
  {
    float percent = pHealth->GetHealthPercent();
    bool alive = pHealth->IsAlive();
    // Update UI elements...
  }
}
```

## How Replication Works Under the Hood

1. When you call `MarkDirty()`, the component is flagged for the next replication tick.
2. During the replication loop, `plNetworkSerializer::SerializePropertiesWithContext()` is called.
3. The serializer checks each property's `plReplicateCondition` and `plReplicateTarget`:
   - `OnChange` properties are compared against a cached last-sent value. If unchanged, they are skipped.
   - `InitialOnly` properties are skipped unless `m_bIsInitialSync` is true.
   - `OwnerOnly` properties are only included when serializing for the owning client.
4. A bitmask is written indicating which properties are included, followed by only those values.
5. On the receiving client, the bitmask is read and only the included properties are deserialized.

## Advanced: Custom Serialization

If the automatic serialization is not sufficient, you can override `NetworkSerialize()`:

```c++
void HealthComponent::NetworkSerialize(plNetworkMessage& msg)
{
  // Let the base class handle attributed properties
  plNetworkComponent::NetworkSerialize(msg);

  // Add custom data that cannot be expressed as simple properties
  msg.Write<plUInt8>(m_uiDamageType);
}

void HealthComponent::NetworkDeserialize(plNetworkMessage& msg)
{
  plNetworkComponent::NetworkDeserialize(msg);
  m_uiDamageType = msg.Read<plUInt8>();
}
```

## Summary

| Concept | What You Learned |
|---------|-----------------|
| Inherit from `plNetworkComponent` | Base class for all replicated components |
| Use `PL_NET_PROPERTY*` macros | Declare properties for automatic serialization |
| Call `MarkDirty()` | Tell the network that state has changed |
| Replication conditions | Control when and to whom properties are sent |
| Client-side `Update()` | React to replicated state for UI and effects |

## See Also

* [Network Component Reference](network-component.md)
* [Network Serialization Reference](network-serialization.md)
* [Getting Started](networking-getting-started.md)

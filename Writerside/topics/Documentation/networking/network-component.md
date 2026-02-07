# Network Component

`plNetworkComponent` is the base class for all components that participate in network replication. It provides the core infrastructure for serialization, dirty tracking, channel configuration, and authority awareness.

## Overview

Any component that needs to replicate state across the network should inherit from `plNetworkComponent`. The base class handles:

* Registration with the `plNetworkWorldModule` on startup.
* Automatic serialization of properties marked with `plNetSerializeAttribute`.
* Dirty flagging so the replication loop knows when to send updates.
* Network role and channel type configuration.
* Ownership and authority queries.

## Inheriting from plNetworkComponent

```c++
class MyNetworkedComponent : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyNetworkedComponent, plNetworkComponent, MyNetworkedComponentManager);

public:
  // Properties you want to replicate
  float m_fHealth = 100.0f;
  plUInt32 m_uiScore = 0;

protected:
  virtual void OnSimulationStarted() override;
  virtual void Update() override;
};
```

In the reflection block, mark properties for replication:

```c++
PL_BEGIN_COMPONENT_TYPE(MyNetworkedComponent, 1, plComponentMode::Static)
{
  PL_BEGIN_PROPERTIES
  {
    PL_NET_PROPERTY("Health", m_fHealth),
    PL_NET_PROPERTY("Score", m_uiScore),
  }
  PL_END_PROPERTIES;
}
PL_END_COMPONENT_TYPE
```

## Serialization

By default, `NetworkSerialize()` and `NetworkDeserialize()` use `plNetworkSerializer` to automatically serialize all properties that have the `plNetSerializeAttribute`. You can override these methods for custom serialization:

```c++
void MyComponent::NetworkSerialize(plNetworkMessage& msg) override
{
  plNetworkComponent::NetworkSerialize(msg);  // Serialize attributed properties
  // Add custom data
  msg.GetWriter().WriteBytes(&m_CustomData, sizeof(m_CustomData));
}

void MyComponent::NetworkDeserialize(plNetworkMessage& msg) override
{
  plNetworkComponent::NetworkDeserialize(msg);
  msg.GetReader().ReadBytes(&m_CustomData, sizeof(m_CustomData));
}
```

## Dirty Tracking

The replication loop only sends updates for components that have been marked dirty. Call `MarkDirty()` whenever a replicated property changes:

```c++
void MyComponent::TakeDamage(float fAmount)
{
  m_fHealth -= fAmount;
  MarkDirty();  // Tell the network to replicate this change
}
```

The replication loop calls `ClearDirty()` after sending the update.

## Network Role

Each component has a network role that determines which machines it is active on:

```c++
pComponent->SetNetworkRole(plNetworkRoleEnum::Server);  // Server-only logic
pComponent->SetNetworkRole(plNetworkRoleEnum::Client);  // Client-only logic
pComponent->SetNetworkRole(plNetworkRoleEnum::Both);    // Active on all machines
```

## Channel Type

Control the delivery guarantee for this component's replication:

```c++
pComponent->SetChannelType(plNetworkChannelTypeEnum::ReliableOrdered);  // Important state
pComponent->SetChannelType(plNetworkChannelTypeEnum::Unreliable);       // Frequent updates
```

## Ownership

Check if the local machine owns this component's game object:

```c++
if (pComponent->IsLocallyOwned())
{
  // This machine is the owner -- apply input, drive state
}
```

## Replication Conditions

If any properties use advanced replication conditions (e.g., `OnChange`, `OwnerOnly`), the component automatically uses the context-aware serialization path:

```c++
// Check at runtime
bool bHasPerRecipient = pComponent->HasPerRecipientProperties();
bool bUsesConditions = pComponent->UsesReplicateConditions();
```

See [Network Serialization](network-serialization.md) for details on replication conditions.

## Network ID

Every registered network component is assigned a unique network ID:

```c++
plUInt32 netID = pComponent->GetNetID();
```

This ID is used internally for message routing and RPC targeting.

## Lifecycle Callbacks

`plNetworkComponent` provides virtual callbacks for low-level connection events:

| Callback | When Called |
|----------|------------|
| `OnNetworkStateChanged(state)` | Connection state changes (connected, disconnected, etc.) |
| `OnClientConnecting(data)` | A client is in the process of connecting |
| `OnClientConnected(pClient)` | A client has successfully connected |
| `OnClientDisconnected(pClient)` | A client has disconnected |

## Network Message Handlers

In addition to the low-level callbacks above, `plNetworkComponent` registers `PL_MESSAGE_HANDLER` entries for all high-level network events. These are delivered through the standard `plMessage` system. Override any of them in your subclass:

| Handler | Message Type | When Called |
|---------|-------------|------------|
| `OnNetworkPlayerJoined` | `plMsgNetworkPlayerJoined` | A player joins the session |
| `OnNetworkPlayerLeft` | `plMsgNetworkPlayerLeft` | A player leaves the session |
| `OnNetworkSessionStateChanged` | `plMsgNetworkSessionStateChanged` | Session state transitions (Lobby, InGame, etc.) |
| `OnNetworkAllPlayersReady` | `plMsgNetworkAllPlayersReady` | All players marked ready |
| `OnNetworkLevelLoadRequested` | `plMsgNetworkLevelLoadRequested` | Server requests a level load |
| `OnNetworkLevelStart` | `plMsgNetworkLevelStart` | Server signals gameplay can begin |
| `OnNetworkAllClientsLoaded` | `plMsgNetworkAllClientsLoaded` | All clients finished level loading |
| `OnNetworkClientConnected` | `plMsgNetworkClientConnected` | A client connects to the server |
| `OnNetworkUserMessage` | `plMsgNetworkUserMessage` | A custom user message (IDs 128-255) is received |
| `OnNetworkValidateSpawn` | `plMsgNetworkValidateSpawn` | Server is about to spawn an object (set `m_bAllowSpawn = false` to reject) |
| `OnNetworkObjectSpawned` | `plMsgNetworkObjectSpawned` | A network object was spawned (server and client) |

Example:

```c++
class MyGameComponent : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyGameComponent, plNetworkComponent, MyGameComponentManager);

  void OnNetworkPlayerJoined(plMsgNetworkPlayerJoined& ref_msg) override
  {
    plLog::Info("Player {} joined", ref_msg.m_uiClientID);
  }

  void OnNetworkLevelStart(plMsgNetworkLevelStart& ref_msg) override
  {
    // Begin gameplay
  }
};
```

All message types are defined in `NetworkPlugin/Core/NetworkMessages.h`.

## See Also

* [Network Serialization](network-serialization.md)
* [Networked Transform Component](networked-transform-component.md)
* [Custom Networked Component Tutorial](networking-custom-component.md)

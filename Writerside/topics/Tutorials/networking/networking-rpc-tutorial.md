# Using RPCs

This tutorial shows how to create and use Remote Procedure Calls (RPCs) to trigger actions across machines. You will define an RPC function, register it, and call it from a client to execute on the server and vice versa.

## Prerequisites

* A working network connection (see [Getting Started](networking-getting-started.md)).
* A custom component inheriting from `plNetworkComponent`.

## What Are RPCs?

RPCs let you call a function on one machine and have it execute on another. Common examples:

* Client tells the server "I want to fire my weapon" (Client -> Server).
* Server tells all clients "Player X was eliminated" (Server -> All Clients).
* Server tells one client "Your inventory updated" (Server -> Owner).

## Step 1: Define the RPC Function

Create a component with the RPC function. The function must be a regular C++ method:

```c++
// MyWeaponComponent.h
class MyWeaponComponent : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyWeaponComponent, plNetworkComponent, MyWeaponComponentManager);

public:
  // Called on the server when a client wants to fire
  void Server_Fire(plVec3 vDirection, float fSpread);

  // Called on all clients when a hit occurs
  void AllClients_OnHit(plVec3 vHitPosition, plUInt32 uiVictimID);
};
```

## Step 2: Implement the Functions

```c++
// MyWeaponComponent.cpp
void MyWeaponComponent::Server_Fire(plVec3 vDirection, float fSpread)
{
  // This runs on the server
  plLog::Info("Client fired weapon! Direction: {}", vDirection);

  // Perform server-side hit detection
  // ...

  // Notify all clients of the hit
  plVariant args[] = { plVariant(hitPos), plVariant(victimID) };
  m_pNetworkModule->GetRpcManager()->CallRpc(
    this, "AllClients_OnHit",
    plArrayPtr<plVariant>(args, 2));
}

void MyWeaponComponent::AllClients_OnHit(plVec3 vHitPosition, plUInt32 uiVictimID)
{
  // This runs on all clients (and server)
  // Spawn hit effect, play sound, update UI
  plLog::Info("Hit at {} on player {}", vHitPosition, uiVictimID);
}
```

## Step 3: Register in Reflection and Register RPCs

Expose the functions via `PL_FUNCTION_PROPERTY` in the reflection block, then register them as RPCs at runtime in `OnSimulationStarted()`:

```c++
PL_BEGIN_COMPONENT_TYPE(MyWeaponComponent, 1, plComponentMode::Static)
{
  PL_BEGIN_FUNCTIONS
  {
    PL_FUNCTION_PROPERTY(Server_Fire, In, "Direction", In, "Spread"),
    PL_FUNCTION_PROPERTY(AllClients_OnHit, In, "HitPosition", In, "VictimID"),
  }
  PL_END_FUNCTIONS;
}
PL_END_COMPONENT_TYPE

void MyWeaponComponent::OnSimulationStarted()
{
  plNetworkComponent::OnSimulationStarted();

  auto* pRpc = m_pNetworkModule->GetRpcManager();

  pRpc->RegisterRpc(GetDynamicRTTI(), "Server_Fire",
    plNetworkRpcTarget::Server, plNetworkRpcReliability::ReliableOrdered);

  pRpc->RegisterRpc(GetDynamicRTTI(), "AllClients_OnHit",
    plNetworkRpcTarget::AllClientsAndServer, plNetworkRpcReliability::ReliableOrdered);
}
```

> **Do not** attach `plNetworkRpcAttribute` to function properties in the reflection block. The editor's phantom RTTI system cannot reconstruct this attribute, which causes a crash during startup. Always use `RegisterRpc()` at runtime instead.

## Step 4: Call the RPC

From the client's input handler (or any code that runs on the owning machine):

```c++
void MyWeaponComponent::OnFireInput()
{
  if (!m_pNetworkModule || !IsLocallyOwned())
    return;

  plVec3 direction = GetOwner()->GetGlobalDirForwards();
  float spread = 0.05f;

  // Using the convenience macro
  PL_CALL_RPC(this, Server_Fire, direction, spread);
}
```

Or using the manager directly:

```c++
m_pNetworkModule->GetRpcManager()->CallRpc(this, "Server_Fire", direction, spread);
```

## Step 5: Multicast to Specific Clients

To send an RPC to only certain clients:

```c++
plDynamicArray<plUInt32> targets;
targets.PushBack(clientID1);
targets.PushBack(clientID2);

plVariant args[] = { plVariant(hitPos), plVariant(victimID) };
pRpcMgr->CallRpc(pComponent, "AllClients_OnHit",
  plArrayPtr<plVariant>(args, 2), targets);
```

## Supported Parameter Types

RPCs support any type that fits in `plVariant`:

* `bool`, `plInt32`, `plUInt32`, `plInt64`, `plUInt64`
* `float`, `double`
* `plString`
* `plVec2`, `plVec3`, `plVec4`
* `plQuat`, `plColor`

## Best Practices

1. **Name RPCs by target** -- Use prefixes like `Server_`, `AllClients_`, `Owner_` to make the target obvious.
2. **Validate on the server** -- Never trust client RPCs blindly. Always validate inputs on the server.
3. **Minimize RPC data** -- Send IDs and indices instead of full objects.
4. **Use reliability wisely** -- Use `ReliableOrdered` for important actions (weapon fire, ability use). Use `Unreliable` for non-critical updates.

## See Also

* [Network RPC Reference](network-rpc.md)
* [Networked Event Component](networked-event-component.md)
* [Getting Started](networking-getting-started.md)

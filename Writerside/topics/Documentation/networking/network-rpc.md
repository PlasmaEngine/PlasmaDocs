# Network RPC System

The RPC (Remote Procedure Call) system allows you to invoke functions on remote machines. It uses Plasma's reflection system for automatic parameter serialization and supports multiple targeting modes and reliability options.

## Overview

RPCs are the primary way to trigger actions across the network -- firing a weapon, applying damage, changing game state, or broadcasting events. The system provides:

* **Reflection-based invocation** -- Functions are invoked through RTTI, with manual registration for target and reliability.
* **Type-safe parameters** -- Arguments are serialized via `plVariant` with type checking.
* **Multiple targets** -- Server-only, owner-only, all clients, or specific clients.
* **Configurable reliability** -- Reliable ordered, reliable, unreliable ordered, or unreliable.

## Accessing the RPC Manager

```c++
plNetworkRpcManager* pRpcMgr = pNetModule->GetRpcManager();
```

## RPC Targets

| Target | Description |
|--------|-------------|
| `Server` | Execute on the server only |
| `Owner` | Execute on the owning client only |
| `AllClients` | Execute on all clients (not the server) |
| `AllClientsAndServer` | Execute on all machines |
| `Multicast` | Execute on a specific list of clients |

## RPC Reliability

| Reliability | Description |
|-------------|-------------|
| `Unreliable` | May be lost |
| `UnreliableOrdered` | May be lost, but in order |
| `Reliable` | Always delivered, may be out of order |
| `ReliableOrdered` | Always delivered, always in order (default) |

## Defining an RPC

An RPC function must be declared as a reflected function property (`PL_FUNCTION_PROPERTY`) so the RPC manager can discover and invoke it through RTTI. The RPC target and reliability are then registered manually at runtime.

### Step 1: Declare the Function

```c++
// Header
class MyComponent : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyComponent, plNetworkComponent, MyComponentManager);
public:
  void Server_ApplyDamage(float fDamage, plUInt32 uiTargetID);
};
```

### Step 2: Reflect as a Function Property

In the reflection block, expose the function via `PL_FUNCTION_PROPERTY`. Do **not** attach `plNetworkRpcAttribute` here -- see the warning below.

```c++
PL_BEGIN_COMPONENT_TYPE(MyComponent, 1, plComponentMode::Static)
{
  PL_BEGIN_FUNCTIONS
  {
    PL_FUNCTION_PROPERTY(Server_ApplyDamage, In, "Damage", In, "TargetID"),
  }
  PL_END_FUNCTIONS;
}
PL_END_COMPONENT_TYPE
```

### Step 3: Register the RPC at Runtime

Register the RPC in `OnSimulationStarted()` using `RegisterRpc()`:

```c++
void MyComponent::OnSimulationStarted()
{
  plNetworkComponent::OnSimulationStarted();

  m_pNetworkModule->GetRpcManager()->RegisterRpc(
    GetDynamicRTTI(),
    "Server_ApplyDamage",
    plNetworkRpcTarget::Server,
    plNetworkRpcReliability::ReliableOrdered);
}
```

## Calling an RPC

### Using Macros (Simplest)

```c++
// From a plNetworkComponent:
PL_CALL_RPC(this, Server_ApplyDamage, 50.0f, targetID);

// From any component with a GetNetID() method:
PL_CALL_RPC_EX(this, Server_ApplyDamage, 50.0f, targetID);
```

### Using the Manager Directly

```c++
// With variadic template (auto-converts to plVariant)
pRpcMgr->CallRpc(pComponent, "Server_ApplyDamage", 50.0f, targetID);

// With explicit variant array
plVariant args[] = { plVariant(50.0f), plVariant(targetID) };
pRpcMgr->CallRpc(pComponent, "Server_ApplyDamage",
  plArrayPtr<plVariant>(args, 2));

// Multicast to specific clients
plDynamicArray<plUInt32> targets;
targets.PushBack(clientID1);
targets.PushBack(clientID2);
pRpcMgr->CallRpc(pComponent, "Server_ApplyDamage",
  plArrayPtr<plVariant>(args, 2), targets);
```

## Macro Reference

| Macro | Description |
|-------|-------------|
| `PL_CALL_RPC(Component, Func, ...)` | Call RPC from a `plNetworkComponent` |
| `PL_CALL_RPC_EX(Component, Func, ...)` | Call RPC from any component with `GetNetID()` |
| `PL_CALL_SERVER_RPC(Component, Func, ...)` | Alias for `PL_CALL_RPC` (semantic clarity) |
| `PL_CALL_SERVER_RPC_EX(Component, Func, ...)` | Alias for `PL_CALL_RPC_EX` |
| `PL_CALL_CLIENT_RPC(Component, Func, ...)` | Alias for `PL_CALL_RPC` |
| `PL_CALL_CLIENT_RPC_EX(Component, Func, ...)` | Alias for `PL_CALL_RPC_EX` |
| `PL_DECLARE_NETWORK_RPC(Func, ...)` | Declare an RPC function signature in a header |

## Supported Parameter Types

RPCs support any type that can be stored in `plVariant`:

* `bool`, `plInt32`, `plUInt32`, `plInt64`, `plUInt64`
* `float`, `double`
* `plString`
* `plVec2`, `plVec3`, `plVec4`
* `plQuat`
* `plColor`

## RPC Execution Flow

1. The caller invokes `CallRpc()` (or uses a macro).
2. The RPC manager serializes the function name hash, component net ID, and arguments into a network message.
3. The message is sent to the appropriate target(s) based on the RPC's target configuration.
4. On the receiving machine, `HandleRpcMessage()` deserializes the message, finds the target component and function, and invokes it via reflection.

## See Also

* [Network Component](network-component.md)
* [Networked Event Component](networked-event-component.md)
* [RPC Tutorial](networking-rpc-tutorial.md)

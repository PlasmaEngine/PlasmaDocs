# Networked Event Component

The `plNetworkedEventComponent` is a lightweight component for broadcasting named events to all clients via reliable RPCs. It is useful for game events that need to reach all machines -- kill feeds, objective updates, sound triggers, or any fire-and-forget notification.

## Overview

Rather than writing custom RPC functions for every game event, you can use this component as a generic event bus:

1. On the authoritative machine (typically the server), call `FireEvent()` with an event name and up to two parameters.
2. The event is broadcast to all clients and the server via a reliable ordered RPC.
3. On each machine, the registered callback is invoked with the event name and parameters.

## Usage

### Firing Events (Server Side)

```c++
auto* pEventComp = pGameObject->GetComponentOfBaseType<plNetworkedEventComponent>();

// Simple event with no parameters
pEventComp->FireEvent("RoundStart");

// Event with parameters
pEventComp->FireEvent("PlayerKilled",
  plVariant(victimID),    // param1
  plVariant(isHeadshot)); // param2
```

### Receiving Events (All Machines)

```c++
pEventComp->SetEventReceivedCallback(
  [](const plString& sEventName, const plVariant& param1, const plVariant& param2) {
    if (sEventName == "PlayerKilled")
    {
      plUInt32 victim = param1.Get<plUInt32>();
      bool headshot = param2.Get<bool>();
      // Update kill feed UI...
    }
    else if (sEventName == "RoundStart")
    {
      // Start countdown...
    }
  });
```

## Supported Parameter Types

The following `plVariant` types can be used as event parameters:

* `Bool`
* `Int32`
* `UInt32`
* `Float`
* `Double`
* `String`
* `Vec3`

Parameters are encoded as type tag + string representation for transport, then decoded on the receiving end.

## Properties

This component has no replicated properties. It uses RPCs exclusively for event delivery. The `NetworkSerialize()` and `NetworkDeserialize()` methods are no-ops.

## Implementation Details

Internally, the component uses a reflected function `AllClients_OnEvent` registered as an RPC with target `AllClientsAndServer` and `ReliableOrdered` reliability. The RPC is registered manually in `OnSimulationStarted()` rather than via reflection attributes to avoid issues with the editor's phantom type system.

## See Also

* [Network RPC System](network-rpc.md)
* [Network Component](network-component.md)

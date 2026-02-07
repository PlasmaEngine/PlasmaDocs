# Networked Rigidbody Component

The `plNetworkedRigidbodyComponent` synchronizes a physics-simulated rigid body across the network. It reads simulation results on the authoritative machine and replicates them to remote clients, where the body is made kinematic and its transform is interpolated.

## Overview

Use this component for any object that uses Jolt physics simulation and needs to be synchronized across the network -- crates, barrels, vehicles, ragdolls, or any dynamic actor.

On the **authoritative machine**, the component reads position, rotation, and velocities from the physics simulation each tick and marks itself dirty for replication. On **remote machines**, the physics actor is switched to kinematic mode and the received state is applied via interpolation.

## Authority Models

The component supports two authority models controlled by the object's `plNetworkObjectRole`:

* **Server authoritative** (`Replicated`) -- The server runs the physics simulation and replicates results. Clients only receive and apply.
* **Owner authoritative** (`OwnedAuthoritative`) -- The owning client runs physics and replicates. Useful for player-controlled physics objects.

```c++
// Check at runtime
if (pRigidbody->HasStateAuthority())  // Can send authoritative updates
if (pRigidbody->HasInputAuthority())  // Can control this object
```

## Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `InterpolationSpeed` | `float` | `10.0` | Speed of position/rotation interpolation on remotes |
| `SyncVelocity` | `bool` | `true` | Include linear velocity in replication |
| `SyncAngularVelocity` | `bool` | `true` | Include angular velocity in replication |
| `TeleportThreshold` | `float` | `5.0` | Snap instead of interpolate above this distance |

## How It Works

### Authority Side

1. `UpdateAsAuthority()` reads the current physics state (transform + velocities) via `ReadPhysicsVelocities()`.
2. The component calls `MarkDirty()` so the replication loop sends the state to clients.

### Remote Side

1. `NetworkDeserialize()` receives the authoritative transform and velocities.
2. `UpdateAsRemote()` interpolates toward the received state at `InterpolationSpeed`.
3. If the distance exceeds `TeleportThreshold`, the position snaps immediately.
4. Received velocities are applied to the kinematic body for visual accuracy.

### Kinematic Switching

On remote machines, the component automatically makes the physics actor kinematic during `OnSimulationStarted()`. This prevents the local physics engine from fighting the replicated state. The actor is restored to dynamic when authority changes (e.g., ownership transfer).

## Custom Serialization

The component overrides `NetworkSerialize()` and `NetworkDeserialize()` to write a compact representation:

* Position (3 floats)
* Rotation (quaternion)
* Linear velocity (3 floats, if `SyncVelocity` is enabled)
* Angular velocity (3 floats, if `SyncAngularVelocity` is enabled)

## Usage

1. Add a Jolt dynamic actor and shape to your prefab.
2. Add `plNetworkedRigidbodyComponent` to the same game object.
3. Spawn the prefab via the [Object Manager](network-object-manager.md).
4. The physics state is automatically replicated.

## See Also

* [Network Component](network-component.md)
* [Networked Transform Component](networked-transform-component.md)
* [Jolt Dynamic Actor](../physics/actors/jolt-dynamic-actor-component.md)

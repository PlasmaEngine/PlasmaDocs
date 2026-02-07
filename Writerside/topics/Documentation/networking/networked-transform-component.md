# Networked Transform Component

The `plNetworkedTransformComponent` replicates a game object's position and rotation across the network with smooth snapshot interpolation. It supports client authority, meaning the owning client drives the transform and broadcasts it to all peers.

## Overview

This component is the primary way to synchronize object positions in a multiplayer game. It is suitable for player characters, NPCs, projectiles, or any moving object that does not use rigid body physics.

On the **authoritative machine** (the owner), the component captures the object's transform each tick and sends it at the configured send rate. On **remote machines**, incoming snapshots are fed into an adaptive-rate interpolator that produces smooth, jitter-free rendering.

No physics plugin dependency is required. For physics-based objects, use [Networked Rigidbody Component](networked-rigidbody-component.md) instead.

## Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `m_fSendRate` | `float` | `20.0` | How many state updates per second to send (Hz) |
| `m_fTeleportThreshold` | `float` | `5.0` | Distance threshold above which the object snaps instead of interpolating |
| `m_bSyncVelocity` | `bool` | `true` | Whether to include derived velocity in state updates |

## How It Works

### Authority Side (Owner)

1. Each frame, `UpdateAsAuthority()` captures the current transform via `CaptureTransformState()`.
2. At the configured `m_fSendRate`, the component writes position, rotation, and velocity into a `TransformState` message and sends it.
3. In host mode, the state is broadcast to all clients. In client mode, it is sent to the host for relay.

### Remote Side (Non-Owner)

1. Incoming `TransformState` messages are received via `HandleTransformStateMessage()`.
2. Each snapshot is pushed into a `plNetworkInterpolator` with a synthetic timestamp for smooth spacing.
3. Each frame, `UpdateAsRemote()` advances the interpolator timeline and calls `ApplyRemotePosition()` and `ApplyRemoteRotation()` to update the game object.

### Teleport Detection

If the distance between the current interpolated position and the next target exceeds `m_fTeleportThreshold`, the component snaps instantly rather than interpolating. This handles respawns, level transitions, or large corrections.

## Virtual Hooks

The component provides virtual methods that subclasses can override for custom behavior:

| Method | Purpose |
|--------|---------|
| `OnAuthorityDetermined(bIsLocal)` | Called once when authority is resolved. Use to set up cameras, input, first/third person, etc. |
| `UpdateAsAuthority()` | Called each frame on the owner. Override to inject input or physics before capturing state. |
| `UpdateAsRemote()` | Called each frame on remotes. Override for custom interpolation or prediction. |
| `CaptureTransformState()` | Reads the current transform into replicated state fields. Override to add custom state. |
| `ApplyRemotePosition(vPosition)` | Applies a received position. Default calls `SetGlobalPosition()`. Override for physics-aware teleports. |
| `ApplyRemoteRotation(qRotation)` | Applies a received rotation. Default calls `SetGlobalRotation()`. |

### Example: Character Controller Override

```c++
class MyCharacterNetTransform : public plNetworkedTransformComponent
{
protected:
  void ApplyRemotePosition(const plVec3& vPosition) override
  {
    // Use character controller teleport instead of direct position set
    m_pCharacterController->RawMove(vPosition - GetOwner()->GetGlobalPosition());
  }
};
```

## Interpolation

The component uses `plNetworkInterpolator` internally, which provides:

* **Adaptive-rate playback** -- Speeds up or slows down slightly to absorb network jitter.
* **Zero extrapolation** -- Holds the last known position rather than predicting, preventing overshoot.
* **Configurable delay** -- Default 100ms buffer for 20 Hz sends.

See [Snapshot Interpolation](network-snapshot-interpolation.md) for details on the interpolation algorithm.

## Usage

1. Add `plNetworkedTransformComponent` to any prefab that should have its transform replicated.
2. Spawn the prefab using the [Object Manager](network-object-manager.md).
3. The owning client's transform is automatically replicated to all other machines.

## See Also

* [Network Component](network-component.md)
* [Networked Rigidbody Component](networked-rigidbody-component.md)
* [Snapshot Interpolation](network-snapshot-interpolation.md)

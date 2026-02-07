# Snapshot Interpolation

The snapshot interpolation system provides smooth rendering of remote entities by buffering transform snapshots and playing them back with an adaptive-rate algorithm. It eliminates jitter, prevents extrapolation artifacts, and handles teleportation gracefully.

## Overview

In a networked game, state updates arrive at irregular intervals due to network jitter. Simply applying each update as it arrives produces visible stuttering. The snapshot interpolation system solves this by:

1. **Buffering** snapshots in a ring buffer.
2. **Maintaining a playback timeline** that runs slightly behind the newest data.
3. **Adapting the playback speed** to absorb jitter: speeding up when the buffer grows, slowing down when it thins.
4. **Interpolating linearly** between the two snapshots bracketing the current timeline position.

The result is smooth, consistent-speed movement with no overshoot or oscillation.

## Key Classes

### plSnapshotBuffer

A templated ring buffer that stores `plNetworkTransformSnapshot` entries and manages the adaptive playback timeline.

```c++
plSnapshotBuffer<16> buffer;  // 16-snapshot ring buffer

// Push a new snapshot
buffer.PushSnapshot(snapshot);

// Advance the timeline each frame
buffer.AdvanceTimeline(frameDt, config);

// Sample the interpolated transform
plTransform transform;
plVec3 velocity;
buffer.SampleAtTimeline(config, transform, &velocity);
```

### plNetworkInterpolator

A convenience wrapper around `plSnapshotBuffer` with a simpler API:

```c++
plNetworkInterpolator interpolator;

// Add a snapshot from the network
interpolator.AddSnapshot(transform, velocity, networkTime, localTime, sequence);

// Each frame, advance and sample
interpolator.Update(frameDt);
plTransform result;
interpolator.GetInterpolatedTransform(networkTime, result);
```

### plSnapshotInterpolationConfig

Configuration for the interpolation behavior:

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `m_InterpolationDelay` | `plTime` | 100 ms | Target delay behind the newest snapshot. Should be at least 2x the send interval. |
| `m_fMaxPlaybackDrift` | `float` | 0.05 | Maximum speed deviation from 1.0x (5%). A character at 3 m/s varies between 2.85 and 3.15 m/s. |
| `m_fPlaybackAdaptSpeed` | `float` | 2.0 | How aggressively the playback rate adapts per second. |
| `m_fTeleportThreshold` | `float` | 5.0 | Distance above which the entity snaps instead of interpolating. |

## How Adaptive-Rate Playback Works

Traditional interpolation picks a fixed render time (e.g., network time minus delay). This is fragile -- if a packet is late, there is nothing to interpolate toward, requiring extrapolation (which overshoots).

The adaptive-rate approach instead controls the **speed** of a local timeline:

1. Calculate how much data is buffered ahead of the timeline.
2. Compare against the target buffer (the `InterpolationDelay`).
3. If too much data is buffered, speed up slightly (drain excess).
4. If too little data is buffered, slow down slightly (buy time for the next packet).
5. Clamp the speed deviation to `MaxPlaybackDrift` to keep movement looking natural.

This produces extremely smooth, consistent-speed movement even under significant jitter.

## Teleport Handling

If the distance between two consecutive snapshots exceeds `TeleportThreshold`, the interpolator snaps to the new position instantly. This handles respawns, level transitions, or large server corrections without producing a visible fast-forward effect.

## Debug Information

Both `plSnapshotBuffer` and `plNetworkInterpolator` expose debug accessors:

```c++
plUInt32 count = interpolator.GetSnapshotCount();   // Snapshots in buffer
plTime delay = interpolator.GetCurrentDelay();       // Effective delay
plTime jitter = interpolator.GetJitter();            // Last measured jitter
float rate = interpolator.GetPlaybackRate();          // Current playback speed
```

Use these with the [Network Debug Component](network-debug-component.md) to visualize interpolation state during development.

## plNetworkTransformSnapshot

A single snapshot in the buffer:

| Field | Type | Description |
|-------|------|-------------|
| `m_Transform` | `plTransform` | Position, rotation, and scale |
| `m_vVelocity` | `plVec3` | Linear velocity at snapshot time |
| `m_vAngularVelocity` | `plVec3` | Angular velocity at snapshot time |
| `m_Timestamp` | `plNetworkTimestamp` | Network time, local time, and sequence number |

## See Also

* [Networked Transform Component](networked-transform-component.md)
* [Networked Rigidbody Component](networked-rigidbody-component.md)

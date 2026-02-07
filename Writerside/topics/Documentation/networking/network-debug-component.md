# Network Debug Component

The `plNetworkDebugComponent` provides in-game visualization of network state for debugging purposes. It renders text overlays showing the network ID, replication status, and network role of the game object.

## Overview

Add this component to any networked game object to see its network information rendered in the viewport. This is useful during development to verify that objects are being replicated correctly, identify authority, and spot replication issues.

## Properties

### Visualization Toggles

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `ShowNetworkId` | `bool` | `true` | Display the object's network ID |
| `ShowReplicationState` | `bool` | `true` | Display whether the component is dirty (pending replication) |
| `ShowNetworkRole` | `bool` | `true` | Display the network role (Server, Client, etc.) |

### Display Settings

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `TextScale` | `float` | `1.0` | Scale of the debug text |
| `TextOffset` | `plVec3` | `(0, 0, 1)` | Offset from the object's position where text is rendered |

### Colors

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `ServerColor` | `plColor` | Lime Green | Color of debug text on the server |
| `ClientColor` | `plColor` | Cornflower Blue | Color of debug text on clients |
| `DirtyColor` | `plColor` | Orange | Color used when the component is dirty |

## Usage

1. Add `plNetworkDebugComponent` to any game object that has a `plNetworkComponent`.
2. Run the game in play mode.
3. Network information is rendered as text overlays above each object.

The component does not replicate any data itself -- it is purely a local visualization tool. Its `NetworkSerialize()` and `NetworkDeserialize()` are no-ops.

## See Also

* [Network Component](network-component.md)
* [Debugging](Debugging.md)

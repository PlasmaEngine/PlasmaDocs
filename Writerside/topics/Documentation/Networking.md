# Networking

The *NetworkPlugin* is an optional engine plugin that provides a complete multiplayer networking solution for Plasma Engine. It handles connection management, state replication, remote procedure calls, object spawning, and session lifecycle.

The plugin uses a client-server architecture backed by [ENet](http://enet.besra.com/) for reliable UDP transport. It supports dedicated servers, listen servers (host mode), and multiple authority models for flexible game design.

## Enable Networking Support

To enable the plugin, use the plugin selection dialog and enable the *NetworkPlugin*. Network functionality is exposed through components, the `plNetworkWorldModule`, and C++ APIs.

## Feature Overview

The networking plugin is composed of several subsystems:

* **[Network World Module](network-world-module.md)** -- The central hub that manages connections, tick rate, and provides access to all other networking subsystems.
* **[Network Components](network-component.md)** -- Base class for components that participate in network replication, plus built-in components for transforms, physics bodies, events, and debugging.
* **[Object Manager](network-object-manager.md)** -- Handles server-authoritative spawning and despawning of prefabs, with object pooling and late-joiner synchronization.
* **[RPC System](network-rpc.md)** -- Type-safe remote procedure calls with reflection-based discovery, multiple targeting modes, and configurable reliability.
* **[Serialization](network-serialization.md)** -- Automatic reflection-based property serialization with quantization, replication conditions, and per-recipient filtering.
* **[Snapshot Interpolation](network-snapshot-interpolation.md)** -- Adaptive-rate playback for smooth remote entity rendering with jitter absorption.
* **[Session Management](network-session.md)** -- High-level session lifecycle with lobby states, ready checks, and player tracking.
* **[Level Manager](network-level-manager.md)** -- Synchronized level loading across all clients with timeout handling and late-joiner support.

For a comprehensive introduction to the architecture and concepts, see the [Networking Overview](networking-overview.md).

## See Also

* [Networking Overview](networking-overview.md)
* [Network Types Reference](network-types.md)

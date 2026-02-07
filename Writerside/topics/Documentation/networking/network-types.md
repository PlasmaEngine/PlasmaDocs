# Network Types

This page documents the core enumerations, structs, and configuration types used throughout the networking plugin.

## plNetworkRoleEnum

Defines the role of the local machine in the network session.

| Value | Description |
|-------|-------------|
| `Undefined` | No role assigned yet |
| `Server` | Dedicated server (no local player) |
| `Client` | Connected to a remote server |
| `Host` | Server and client combined (listen server) |
| `Both` | Alias for Host |

## plNetworkModeEnum

High-level network mode.

| Value | Description |
|-------|-------------|
| `Offline` | No networking active |
| `Client` | Running as a client |
| `Server` | Running as a server |

## plNetworkChannelTypeEnum

Controls the delivery guarantee for a message or component replication.

| Value | Description |
|-------|-------------|
| `None` | Invalid channel |
| `Unreliable` | Message may be lost or arrive out of order |
| `UnreliableOrdered` | Message may be lost but will arrive in order |
| `Reliable` | Message will always be received but may be out of order |
| `ReliableOrdered` | Message will always be received and will be in order |

**Guidance:** Use `Unreliable` for frequent state updates (transforms, positions) where only the latest value matters. Use `ReliableOrdered` for important events (RPCs, spawn/despawn, game state changes).

## plNetworkObjectRole

Defines the authority model for a networked object.

| Value | Description |
|-------|-------------|
| `None` | Not a networked object |
| `OwnedAuthoritative` | The owning client has full authority over this object |
| `Replicated` | The server has authority; clients receive read-only state |
| `ReplicatedSimulated` | Server-authoritative with client-side prediction |

## plNetworkConnectionState

The connection lifecycle state.

| Value | Description |
|-------|-------------|
| `Offline` | Not connected |
| `Connecting` | Connection attempt in progress |
| `Connected` | Successfully connected |
| `Disconnecting` | Disconnect in progress |
| `Disconnected` | Connection terminated |

## plNetworkDisconnectReason

Reason codes for disconnection, used with `Stop()` and `KickClient()`.

| Value | Description |
|-------|-------------|
| `Unknown` | No specific reason |
| `ClientQuit` | Client initiated graceful disconnect |
| `ServerShutdown` | Server is shutting down |
| `Kicked` | Client was kicked by the server |
| `Timeout` | Connection timed out |
| `VersionMismatch` | Protocol or game version mismatch |
| `AuthenticationFailed` | Authentication failure |
| `ServerFull` | Server has no available slots |
| `RateLimited` | Client exceeded rate limits |
| `Banned` | Client is banned |

## plNetworkConfig

Configuration struct for network connections. Set this on the `plNetworkWorldModule` before calling `StartServer()`, `StartClient()`, or `StartHost()`.

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `m_DriverType` | `plDriverTypeEnum` | `ENet` | Network transport driver |
| `m_uiConnectionLimit` | `plUInt16` | `32` | Maximum number of connections |
| `m_sServerAddress` | `plString` | `"127.0.0.1"` | Server address to connect to |
| `m_uiServerPort` | `plUInt16` | `7777` | Server port |
| `m_uiMessageSize` | `plUInt16` | `1500` | Maximum message size in bytes |
| `m_uiMessagePoolSize` | `plUInt16` | `2048` | Size of the internal message pool |

## plNetworkMessageIDs

Defines the message ID ranges for the network protocol.

### Core Protocol (0 - 63)

| ID | Name | Description |
|----|------|-------------|
| 0 | `Undefined` | Invalid |
| 1 | `Handshake` | Client connection request |
| 2 | `HandshakeReply` | Server response to handshake |
| 3 | `ObjectReplicate` | Component state replication |
| 4 | `ObjectReplicatePart` | Partial replication (large objects) |
| 5 | `ObjectSpawn` | Spawn a networked object |
| 6 | `ObjectSpawnPart` | Partial spawn data |
| 7 | `ObjectDespawn` | Despawn a networked object |
| 8 | `ObjectRole` | Authority/ownership change |
| 9 | `ObjectRpc` | Remote procedure call |
| 10 | `TimeSync` | Client requests time synchronization |
| 11 | `TimeSyncResponse` | Server time sync response |
| 12 | `Disconnect` | Graceful disconnect with reason |
| 13 | `Reconnect` | Client reconnection attempt |
| 14 | `ReconnectResponse` | Server reconnection response |
| 15 | `ServerRewind` | Lag compensation rewind request |
| 16 | `LevelLoad` | Server tells clients to load a level |
| 17 | `LevelLoadComplete` | Client reports level load finished |
| 18 | `LevelStart` | Server signals gameplay can begin |

### Engine Component Messages (64 - 127)

Reserved for built-in engine component communication.

| ID | Name | Description |
|----|------|-------------|
| 64 | `TransformState` | Replicated transform state (used by `plNetworkedTransformComponent`) |

### User/Game Messages (128 - 255)

Reserved for game-specific messages. Use `plNetworkMessageIDs::UserMessageStart` (128) as the starting point for your custom message IDs, and register a handler via `SetUserMessageCallback()` on the world module.

## plNetworkConnection

Represents a network connection with a unique ID:

```c++
struct plNetworkConnection
{
  plUInt32 m_uiConnectionID;
};
```

## plNetworkStats

Network statistics for a connection:

| Field | Type | Description |
|-------|------|-------------|
| `m_fRountTripTime` | `float` | Current round-trip time in seconds |
| `m_uiPacketsLost` | `plUInt32` | Packets lost in the current period |
| `m_uiTotalPacketsSent` | `plUInt64` | Total packets sent since connection |
| `m_uiTotalPacketsLost` | `plUInt32` | Total packets lost since connection |
| `m_uiTotalBytesSent` | `plUInt64` | Total bytes sent |
| `m_uiTotalBytesReceived` | `plUInt64` | Total bytes received |

## See Also

* [Networking Overview](networking-overview.md)
* [Network World Module](network-world-module.md)

# Network World Module

The `plNetworkWorldModule` is the central networking hub. It is a [world module](../world-modules.md) that manages connections, processes messages, runs the replication loop, and provides access to all networking subsystems.

## Accessing the Module

```c++
plNetworkWorldModule* pNetModule = pWorld->GetModule<plNetworkWorldModule>();
```

The module is automatically available in any world where the NetworkPlugin is loaded.

## Starting the Network

Before starting, configure the network settings:

```c++
plNetworkConfig config;
config.m_sServerAddress = "192.168.1.100";
config.m_uiServerPort = 7777;
config.m_uiConnectionLimit = 16;

pNetModule->SetNetworkConfig(config);
```

Then start in one of three modes:

* `StartServer()` -- Start as a dedicated server (no local player).
* `StartClient()` -- Connect to a remote server.
* `StartHost()` -- Start as both server and client (listen server).

```c++
// Dedicated server
pNetModule->StartServer();

// Client
pNetModule->StartClient();

// Listen server (host)
pNetModule->StartHost();
```

## Stopping the Network

```c++
// Graceful disconnect with reason
pNetModule->Stop(plNetworkDisconnectReason::ClientQuit);

// Kick a specific client (server only)
pNetModule->KickClient(clientID, plNetworkDisconnectReason::Kicked);
```

## State Queries

| Method | Returns |
|--------|---------|
| `IsServer()` | True if running as server |
| `IsClient()` | True if running as client |
| `IsHost()` | True if running as host (server + client) |
| `IsConnected()` | True if connection is established |
| `IsOffline()` | True if disconnected or offline |
| `GetRole()` | Current `plNetworkRoleEnum` value |
| `GetStatus()` | Current `plNetworkConnectionState` |
| `GetLocalClientID()` | This machine's client ID |
| `GetServerClientID()` | The server's client ID |

## Sub-Manager Accessors

All subsystems are owned by the world module and accessed through getters:

```c++
plNetworkObjectManager*    pNetModule->GetObjectManager();
plNetworkRpcManager*       pNetModule->GetRpcManager();
plNetworkBandwidthManager* pNetModule->GetBandwidthManager();
plNetworkTime*             pNetModule->GetNetworkTime();
plNetworkLagCompensation*  pNetModule->GetLagCompensation();
plNetworkLevelManager*     pNetModule->GetLevelManager();
plNetworkSession*          pNetModule->GetSession();
```

## Tick Rate

The network tick rate controls how often the replication loop runs:

```c++
pNetModule->SetTickRate(60.0f);  // Default: 60 Hz
float rate = pNetModule->GetTickRate();
```

## Authority Validation

The module provides helpers for checking whether the local machine or a specific client has authority over a component:

```c++
// Check if a specific client has authority
bool bHasAuth = pNetModule->HasAuthority(pComponent, clientID);

// Check if the local machine has authority
bool bLocalAuth = pNetModule->HasLocalAuthority(pComponent);

// Validate an incoming state update from a sender
bool bValid = pNetModule->ValidateStateUpdate(componentNetID, senderClientID);
```

## Client Management

```c++
// Get all connected clients
plDynamicArray<plNetworkClient*>& clients = pNetModule->GetClients();

// Look up a specific client
plNetworkClient* pClient = pNetModule->GetClient(clientID);
```

## Rate Limiting

Protect the server from message floods:

```c++
// Max 1000 messages per second per client (0 = no limit)
pNetModule->SetRateLimit(1000);

// Kick after 5 violations (0 = never kick)
pNetModule->SetMaxRateLimitViolations(5);
```

## Network Message Handlers

The world module broadcasts network events as `plMessage` types to all registered `plNetworkComponent` subclasses. Override the handlers in your component to react to them.

### User Messages

Custom game messages (IDs 128-255) are delivered as `plMsgNetworkUserMessage`:

```c++
void MyGameComponent::OnNetworkUserMessage(plMsgNetworkUserMessage& ref_msg) override
{
  if (ref_msg.m_uiMessageID == 128)
  {
    // Handle custom message using ref_msg.m_pNetworkMessage
  }
}
```

### Client Connected

Get notified when a new client connects:

```c++
void MyGameComponent::OnNetworkClientConnected(plMsgNetworkClientConnected& ref_msg) override
{
  plLog::Info("Client {} connected", ref_msg.m_uiClientID);
}
```

### Message Broadcasting

The world module provides a helper used internally by Session, LevelManager, and the module itself:

```c++
void plNetworkWorldModule::BroadcastToNetworkComponents(plMessage& ref_msg);
```

This iterates all registered `plNetworkComponent` instances and calls `SendMessage()` on their owning game objects, routing the message through the standard `PL_MESSAGE_HANDLER` system.

## Convenience Time Methods

```c++
// Get the synchronized network time
plTime syncedTime = pNetModule->GetSyncedTime();

// Get the round-trip time to the server
plTime rtt = pNetModule->GetRTT();
```

## Component and Object Registration

Network components and objects are registered automatically when they start up. Manual registration is available for advanced use:

```c++
pNetModule->RegisterNetworkComponent(pComponent);
pNetModule->RemoveNetworkComponent(pComponent);

pNetModule->RegisterNetworkObject(pNetObject);
pNetModule->RemoveNetworkObject(pNetObject);
```

## Game Version

Set a game version to prevent clients with mismatched versions from connecting:

```c++
pNetModule->SetGameVersion(1);
```

The version is validated during the handshake. A mismatch results in a rejected connection.

## See Also

* [Networking Overview](networking-overview.md)
* [Network Types](network-types.md)
* [Getting Started Tutorial](../../Tutorials/networking/networking-getting-started.md)

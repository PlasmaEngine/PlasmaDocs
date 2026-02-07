# Network Object Manager

The `plNetworkObjectManager` handles server-authoritative spawning and despawning of prefabs across the network. It tracks ownership, authority, and provides object pooling for frequently spawned objects.

## Overview

In a multiplayer game, the server decides when and where objects appear. The Object Manager:

1. **Registers** prefabs that can be spawned over the network.
2. **Spawns** prefab instances on the server and automatically replicates the spawn to all clients.
3. **Tracks** ownership and authority for each spawned object.
4. **Despawns** objects on the server and replicates the despawn to all clients.
5. **Synchronizes** existing objects to late-joining clients.
6. **Pools** objects for efficient reuse.

## Accessing the Manager

```c++
plNetworkObjectManager* pObjMgr = pNetModule->GetObjectManager();
```

## Prefab Registration

Before a prefab can be spawned, it must be registered:

```c++
plHashedString sPrefab = plMakeHashedString("Player.plPrefab");
pObjMgr->RegisterNetworkPrefab(sPrefab);

// Optional: assign a numeric ID for smaller network messages
pObjMgr->RegisterNetworkPrefab(sPrefab, 1);
```

Unregister when no longer needed:

```c++
pObjMgr->UnregisterNetworkPrefab(sPrefab);
```

Check if a prefab is registered:

```c++
bool bRegistered = pObjMgr->IsNetworkPrefab(sPrefab);
```

## Spawning Objects

Spawn a networked object on the server. The spawn is automatically replicated to all clients:

```c++
plTransform spawnTransform;
spawnTransform.m_vPosition = plVec3(0, 0, 1);
spawnTransform.m_qRotation = plQuat::MakeIdentity();

plUInt32 uiNetID = pObjMgr->SpawnNetworkObject(
  sPrefab,
  spawnTransform,
  ownerClientID,                       // 0 = server-owned
  plNetworkObjectRole::OwnedAuthoritative);
```

Spawn as a child of another object:

```c++
plUInt32 uiNetID = pObjMgr->SpawnNetworkObject(
  sPrefab,
  localTransform,
  hParentObject,
  ownerClientID,
  plNetworkObjectRole::OwnedAuthoritative);
```

The returned `uiNetID` is the unique network identifier for the spawned object, consistent across all machines.

## Despawning Objects

```c++
pObjMgr->DespawnNetworkObject(uiNetID);
```

Despawn all objects owned by a specific client (useful on disconnect):

```c++
pObjMgr->DespawnObjectsOwnedBy(clientID);
```

## Ownership and Authority

### Transfer Ownership

```c++
pObjMgr->TransferOwnership(uiNetID, newOwnerClientID);
```

### Change Authority

```c++
pObjMgr->SetAuthority(uiNetID, plNetworkObjectRole::Replicated);
```

### Query Ownership

```c++
plUInt32 owner = pObjMgr->GetOwner(uiNetID);
plNetworkObjectRole::Enum auth = pObjMgr->GetAuthority(uiNetID);
bool bHasAuth = pObjMgr->HasAuthority(uiNetID, clientID);
```

## Object Pooling

For frequently spawned and despawned objects (projectiles, effects), enable pooling to avoid instantiation overhead:

```c++
// Pre-allocate 20 instances of the projectile prefab
pObjMgr->EnablePooling(sPrefab, 20);
```

When pooling is enabled:

* `SpawnNetworkObject()` reuses a pooled instance instead of creating a new one.
* `DespawnNetworkObject()` deactivates and returns the object to the pool instead of destroying it.

Query pool state:

```c++
bool bPooled = pObjMgr->IsPoolingEnabled(sPrefab);
plUInt32 available = pObjMgr->GetPooledCount(sPrefab);
```

## Object Lookup

```c++
// Get object info by network ID
const plNetworkObjectInfo* pInfo = pObjMgr->GetObjectInfo(uiNetID);

// Get the game object handle for a network ID
plGameObjectHandle hObject = pObjMgr->GetGameObject(uiNetID);

// Get the network ID for a game object
plUInt32 id = pObjMgr->GetNetworkID(hObject);

// Iterate all tracked network objects
const auto& allObjects = pObjMgr->GetAllObjects();
```

## Spawn Messages

Spawn lifecycle events are delivered as `plMessage` types to all registered `plNetworkComponent` subclasses, following the same pattern as session and level events. Override the handlers in your component.

### Spawn Validation

Before a server-side spawn is executed, a `plMsgNetworkValidateSpawn` is broadcast. Any handler can reject the spawn by setting `m_bAllowSpawn = false`. Because `SendMessage` is synchronous, the result is available immediately -- if any component rejects, the spawn is cancelled and no network traffic is sent:

```c++
void MySpawnGuard::OnNetworkValidateSpawn(plMsgNetworkValidateSpawn& ref_msg) override
{
  // Only allow players to spawn their own character
  if (ref_msg.m_sPrefabGuid != plMakeHashedString("Player.plPrefab"))
  {
    ref_msg.m_bAllowSpawn = false;
  }
}
```

### Post-Spawn Notification

After an object is spawned (on both server and clients receiving replicated spawns), a `plMsgNetworkObjectSpawned` is broadcast with the newly created game object:

```c++
void MyGameManager::OnNetworkObjectSpawned(plMsgNetworkObjectSpawned& ref_msg) override
{
  ref_msg.m_pSpawnedObject->SetName(plFmt("Player_{}", ref_msg.m_uiOwnerClientID));
  // Set team color, initial loadout, etc.
}
```

## Late-Joiner Synchronization

When a new client connects, call `SyncAllObjectsToClient()` to send the full state of all existing objects:

```c++
pObjMgr->SyncAllObjectsToClient(clientID);
```

This is handled automatically by the `plNetworkWorldModule` during the handshake process.

## plNetworkObjectInfo

Each tracked object has associated metadata:

| Field | Type | Description |
|-------|------|-------------|
| `m_uiNetworkID` | `plUInt32` | Unique network identifier |
| `m_hGameObject` | `plGameObjectHandle` | Handle to the game object |
| `m_uiOwnerClientID` | `plUInt32` | Client that owns this object |
| `m_Authority` | `plNetworkObjectRole` | Authority level |
| `m_sPrefabGuid` | `plHashedString` | Prefab used to spawn |
| `m_SpawnTime` | `plTime` | When the object was spawned |
| `m_bPendingDestroy` | `bool` | Marked for destruction |

## See Also

* [Network World Module](network-world-module.md)
* [Spawning Objects Tutorial](../../Tutorials/networking/networking-spawning-objects.md)

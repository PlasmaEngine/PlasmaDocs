# Spawning Networked Objects

This tutorial shows how to spawn and despawn prefabs across the network using the `plNetworkObjectManager`. You will learn to register prefabs, spawn player characters, handle ownership, and use object pooling.

## Prerequisites

* A working network connection (see [Getting Started](networking-getting-started.md)).
* A prefab to spawn (e.g., a player character or a projectile).

## Step 1: Register a Prefab

Before a prefab can be spawned over the network, it must be registered with the Object Manager. Do this during initialization:

```c++
auto* pObjMgr = pNetModule->GetObjectManager();

// Register prefabs by their asset GUID or path
plHashedString sPlayerPrefab = plMakeHashedString("Player.plPrefab");
pObjMgr->RegisterNetworkPrefab(sPlayerPrefab);

plHashedString sProjectilePrefab = plMakeHashedString("Projectile.plPrefab");
pObjMgr->RegisterNetworkPrefab(sProjectilePrefab);
```

## Step 2: Spawn a Player on Connection

When a client connects, spawn a player character owned by that client. Create a component that handles the `plMsgNetworkClientConnected` message:

```c++
class MyPlayerSpawner : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyPlayerSpawner, plNetworkComponent, MyPlayerSpawnerManager);

  void OnNetworkClientConnected(plMsgNetworkClientConnected& ref_msg) override
  {
    if (!IsHostOrServer())
      return;  // Only spawn on the server

    auto* pObjMgr = m_pNetworkModule->GetObjectManager();
    plHashedString sPrefab = plMakeHashedString("Player.plPrefab");

    plTransform spawnPos;
    spawnPos.m_vPosition = plVec3(0, 0, 1);  // Spawn location
    spawnPos.m_qRotation = plQuat::MakeIdentity();

    plUInt32 netID = pObjMgr->SpawnNetworkObject(
      sPrefab,
      spawnPos,
      ref_msg.m_uiClientID,                     // Owner = the connecting client
      plNetworkObjectRole::OwnedAuthoritative);  // Client has authority

    plLog::Info("Spawned player {} for client {}", netID, ref_msg.m_uiClientID);
  }
};
```

The Object Manager automatically:
- Creates the prefab on the server.
- Sends a spawn message to all clients.
- Assigns the network ID to all `plNetworkComponent` instances on the prefab.
- Late-joining clients receive spawn messages for all existing objects.

## Step 3: Despawn on Disconnect

Clean up when a client disconnects:

```c++
// Option 1: Despawn all objects owned by the client
pObjMgr->DespawnObjectsOwnedBy(clientID);

// Option 2: Despawn a specific object
pObjMgr->DespawnNetworkObject(netID);
```

## Step 4: Spawn Projectiles

For frequently spawned objects like projectiles, the flow is similar but typically triggered by gameplay:

```c++
void MyWeaponComponent::FireProjectile()
{
  auto* pNetModule = GetWorld()->GetModule<plNetworkWorldModule>();
  auto* pObjMgr = pNetModule->GetObjectManager();

  plHashedString sPrefab = plMakeHashedString("Projectile.plPrefab");

  plTransform spawnPos = GetOwner()->GetGlobalTransform();

  plUInt32 netID = pObjMgr->SpawnNetworkObject(
    sPrefab,
    spawnPos,
    0,                                     // Server-owned
    plNetworkObjectRole::Replicated);      // Server-authoritative

  // Optionally customize via post-spawn callback
}
```

## Step 5: Enable Object Pooling

For projectiles and effects that spawn and despawn frequently, enable pooling to avoid instantiation overhead:

```c++
plHashedString sPrefab = plMakeHashedString("Projectile.plPrefab");

// Pre-allocate 50 instances
pObjMgr->EnablePooling(sPrefab, 50);
```

With pooling enabled:

- `SpawnNetworkObject()` reuses a pooled (deactivated) instance instead of instantiating.
- `DespawnNetworkObject()` deactivates and returns the object to the pool instead of destroying it.

Check pool status:

```c++
bool pooled = pObjMgr->IsPoolingEnabled(sPrefab);
plUInt32 available = pObjMgr->GetPooledCount(sPrefab);
```

## Step 6: Transfer Ownership

You can transfer ownership of an object to a different client at runtime:

```c++
// Give the vehicle to Client 3
pObjMgr->TransferOwnership(vehicleNetID, 3);
```

This updates the authority and notifies all machines of the change.

## Step 7: Post-Spawn Customization

Override `OnNetworkObjectSpawned` in a `plNetworkComponent` subclass to customize objects after they are spawned:

```c++
void MyGameManager::OnNetworkObjectSpawned(plMsgNetworkObjectSpawned& ref_msg) override
{
  ref_msg.m_pSpawnedObject->SetName(plFmt("Player_{}", ref_msg.m_uiOwnerClientID));

  // Set team color, initial loadout, etc.
}
```

## Complete Example

Register prefabs during game state activation, then handle spawning via a component:

```c++
// In your game state (initialization):
void MyGameState::OnActivation(plWorld* pWorld)
{
  plGameState::OnActivation(pWorld);

  auto* pNetModule = pWorld->GetModule<plNetworkWorldModule>();
  auto* pObjMgr = pNetModule->GetObjectManager();

  // Register prefabs
  pObjMgr->RegisterNetworkPrefab(plMakeHashedString("Player.plPrefab"));
  pObjMgr->RegisterNetworkPrefab(plMakeHashedString("Projectile.plPrefab"));

  // Pool projectiles
  pObjMgr->EnablePooling(plMakeHashedString("Projectile.plPrefab"), 50);
}
```

```c++
// In a networked component (spawn and cleanup):
class MyPlayerManager : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyPlayerManager, plNetworkComponent, MyPlayerManagerManager);

  void OnNetworkClientConnected(plMsgNetworkClientConnected& ref_msg) override
  {
    if (!IsHostOrServer())
      return;

    auto* pObjMgr = m_pNetworkModule->GetObjectManager();

    plTransform spawnPos;
    spawnPos.m_vPosition = GetSpawnPoint(ref_msg.m_uiClientID);
    spawnPos.m_qRotation = plQuat::MakeIdentity();

    pObjMgr->SpawnNetworkObject(
      plMakeHashedString("Player.plPrefab"),
      spawnPos, ref_msg.m_uiClientID,
      plNetworkObjectRole::OwnedAuthoritative);
  }

  void OnNetworkPlayerLeft(plMsgNetworkPlayerLeft& ref_msg) override
  {
    if (!IsHostOrServer())
      return;

    // Clean up disconnected player's objects
    m_pNetworkModule->GetObjectManager()->DespawnObjectsOwnedBy(ref_msg.m_uiClientID);
  }
};
```

## See Also

* [Network Object Manager Reference](../../Documentation/networking/network-object-manager.md)
* [Getting Started](networking-getting-started.md)
* [Network Component](../../Documentation/networking/network-component.md)

# Getting Started with Networking

This tutorial walks you through setting up a basic multiplayer connection in Plasma Engine, from enabling the plugin to verifying replication with the debug component.

## Prerequisites

* A Plasma Engine project with a C++ game plugin.
* The project should be able to compile and run a basic scene.

## Step 1: Enable the Network Plugin

Open your project in the Plasma Editor. Go to **Project > Plugin Selection** and enable the **NetworkPlugin**. This makes all networking components and the `plNetworkWorldModule` available. The engine handles linking automatically -- no changes to your `CMakeLists.txt` are needed.

Include the main header in your game code:

```c++
#include <NetworkPlugin/WorldModule/NetworkWorldModule.h>
```

## Step 2: Configure and Start the Network

The best place to start the network is in your `plGameState` or a startup component. Here is a minimal example using a game state:

```c++
#include <NetworkPlugin/WorldModule/NetworkWorldModule.h>

class MyGameState : public plGameState
{
  PL_ADD_DYNAMIC_REFLECTION(MyGameState, plGameState);

public:
  void OnActivation(plWorld* pWorld) override
  {
    plGameState::OnActivation(pWorld);

    auto* pNetModule = pWorld->GetModule<plNetworkWorldModule>();
    if (!pNetModule)
      return;

    // Configure the network
    plNetworkConfig config;
    config.m_sServerAddress = "127.0.0.1";
    config.m_uiServerPort = 7777;
    config.m_uiConnectionLimit = 4;

    pNetModule->SetNetworkConfig(config);
    pNetModule->SetGameVersion(1);

    // Start as server or client based on a command-line flag or config
    if (m_bIsServer)
    {
      pNetModule->StartHost();  // Host = server + local player
      plLog::Info("Started as Host on port {}", config.m_uiServerPort);
    }
    else
    {
      pNetModule->StartClient();
      plLog::Info("Connecting to {}:{}", config.m_sServerAddress, config.m_uiServerPort);
    }
  }

private:
  bool m_bIsServer = true;
};
```

## Step 3: Verify the Connection

To verify the connection is working, create a simple networked component that logs connection events:

```c++
#include <NetworkPlugin/Components/NetworkComponent.h>

class MyConnectionLogger : public plNetworkComponent
{
  PL_DECLARE_COMPONENT_TYPE(MyConnectionLogger, plNetworkComponent, MyConnectionLoggerManager);

  void OnNetworkClientConnected(plMsgNetworkClientConnected& ref_msg) override
  {
    plLog::Success("Client {} connected!", ref_msg.m_uiClientID);
  }
};
```

Add this component to an object in your scene. Run two instances of your game -- one as a host and one as a client. You should see the connection messages in the log.

## Step 4: Add a Debug Component

To visualize network state in the viewport:

1. Create a simple prefab with a mesh (e.g., a sphere).
2. Add a `plNetworkComponent` to the root object.
3. Add a `plNetworkDebugComponent` to the same object.
4. Place the prefab in your scene.

When you run the game, you will see debug text above the object showing its network ID, replication state, and network role.

## Step 5: Check Network State at Runtime

You can query the network state from any component or game state:

```c++
auto* pNetModule = GetWorld()->GetModule<plNetworkWorldModule>();

if (pNetModule->IsConnected())
{
  plLog::Info("Connected as {} (Client ID: {})",
    pNetModule->IsServer() ? "Server" : "Client",
    pNetModule->GetLocalClientID());

  plLog::Info("RTT: {:.1f}ms", pNetModule->GetRTT().GetMilliseconds());
}
```

## Next Steps

Now that you have a working connection:

* **[Spawn networked objects](networking-spawning-objects.md)** -- Learn to spawn prefabs that replicate across the network.
* **[Use RPCs](networking-rpc-tutorial.md)** -- Trigger actions on remote machines.
* **[Build a custom component](networking-custom-component.md)** -- Create a replicated health component.

## See Also

* [Networking Overview](networking-overview.md)
* [Network World Module](network-world-module.md)

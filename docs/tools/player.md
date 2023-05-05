# plPlayer

The plPlayer is a stand-alone application that can run any Plasma Engine game that is properly embedded in its own DLL. The plEditor can [launch a scene](../editor/run-scene.md) directly in the plPlayer application. The plPlayer is meant for testing and as a very slim example of how to write a custom game application.

## Arguments

The Player takes these command line arguments:

```cmd
Player.exe -project "ProjectPath" -scene "ScenePath" [-wnd "optional/path/to/Window.ddl"] [-profile "OptionalAssetProfileName"]
```

With:

* `ProjectPath`: The absolute path to the project directory.
* `ScenePath`: A relative path to a scene file. It is relative to the [data directory](../projects/data-directories.md) that it resides in. If it is a path to an `.plScene` or `.plPrefab` file, plPlayer automatically redirects the path to the corresponding exported `.plObjectGraph` file in the *AssetCache*.

Typically you only need to pass the path to the project and scene (or prefab) file. The other options are used by the [plEditor](../../getting-started/editor-overview.md) to select different configurations.

## Execution

The Player will automatically detect the [projects](../projects/projects-overview.md) directory by searching the file system for an plProject file. It then executes the core Plasma Engine functionality, meaning it reads the configuration for the [data directories](../projects/data-directories.md) as well as the [engine plugins](../custom-code/cpp/engine-plugins.md) from the project config files. If the scene requires custom (game) plugins, they must be referenced in those config files.

Then it will execute the regular game loop. Thus, if the scene contains game objects to spawn a character controller or otherwise handle input and move the camera, you will be able to interact with it. If a custom [plugin](../custom-code/cpp/engine-plugins.md) implements a custom [game state](../runtime/application/game-state.md) that will be instantiated and can take full control over the application logic. If no such functionality is available, the Player will instantiate the `plFallbackGameState` which will spawn a player object, if a `plPlayerStartPointComponent` is part of the scene. Otherwise it will provide a simple WASD camera movement scheme. If `plCameraComponent`s are placed in the scene, you can cycle through them using `Page Up` and `Page Down`.

Pressing **Escape** will close the Player application (unless overridden by a custom game state).

## Common Application Features

Since plPlayer is built on the [application (TODO)](../runtime/application/application.md) framework, it provides a set of useful features common to all Plasma applications.

See [this page](../runtime/application/common-application-features.md) for details.

## See Also

* [Game States](../runtime/application/game-state.md)
* [Engine Plugins](../custom-code/cpp/engine-plugins.md)
* [Projects](../projects/projects-overview.md)
* [plEditor Overview](../../getting-started/editor-overview.md)

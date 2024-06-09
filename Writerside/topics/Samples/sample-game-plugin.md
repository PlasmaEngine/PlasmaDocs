# Sample Game Plugin

The **SampleGamePlugin** demonstrates the basics of how to build a [custom plugin](Code.md) for game code that can run both in a stand-alone application (such as [plPlayer](player.md)) as well as inside the editor.

## Prerequisites

> **Note:**
>
> The project is only available when the solution is built with **PL_BUILD_SAMPLES** activated.

## GameState

The *SampleGameState* class shows how to implement a simple [game state](game-state.md) that adds high-level game logic, such as handling a game UI. See `plGameState` and `plGameApplication` for further details.

## Components

* The `DemoComponent` shows how to modify the transform of an object dynamically.

* The `DebugRenderComponent` shows how to use [debug rendering](debug-rendering.md).

For further details also see `plComponent`.

## Project

Under *Data/Samples/SampleGame* you will find an [editor project](projects-overview.md) which uses the `SampleGamePlugin`. Note that the project references the plugin as a [runtime plugin](engine-plugins.md) (under *Project > [Plugin Settings](project-settings.md) > Plugin Selection...*). This makes the custom components available to the editor.

When you press 'Play' in the editor, the scene will be simulated and the custom components, such as the `DemoComponent`, will take effect.

When you press 'Play the Game' a full game window is launched and now even the custom [game state](game-state.md) is instantiated and executed. Consequently, the UI will appear and you can interact with it. Note that this still runs inside the editor process.

You can also [export and run the scene](run-scene.md) externally in the stand-alone [plPlayer](player.md) application.

## See Also

* [Samples](Samples.md)
* [Running a Scene](run-scene.md)
* [Game States](game-state.md)
* [Custom Code](Code.md)
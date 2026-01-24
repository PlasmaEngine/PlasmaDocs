# Common Application Features

All applications that are built on top of `plGameApplication` provide a number of useful features for developers.

## In-game console

**Press F1** to toggle the in-game [console](console.md). See its documentation for further details.

## Reload Resources

**Press F4** to instruct the engine to reload all [resources (TODO)](resource-management.md). This can be useful, if for example, you are working on a [shader (TODO)](Shaders.md) and want to see the result of your changes inside the game, without having to restart the game.

Reloading resources works for all assets that are used directly by the engine (e.g. [shaders (TODO)](Shaders.md)). For some assets it will work, after the editor processed the input [assets](assets-overview.md). For example for [textures](textures-overview.md) and [materials](materials-overview.md) and many others. Some resources, though, are not reloadable, e.g. things that get instantiated at runtime, such as [prefabs](../../prefabs/prefabs-overview.md).

## Show Frames Per Second

**Press F5** to toggle the display of the FPS counter.

## Take a Profiling Capture

**Press F8** to take a capture of the profiling data. See the [profiling](profiling.md) documentation for details.

## Take a RenderDoc Capture

**Press F11** to take a RenderDoc capture. See the [RenderDoc integration](renderdoc.md) documentation for details.

## Take a Screenshot

**Press F12** to take a screenshot. Screenshots are stored in the `appdata` [data directory](data-directories.md) (see the [log output](logging.md)). On Windows this can be found by typing `%appdata%` into the Windows Explorer.

## See Also


* [Application (TODO)](application.md)
* [Player](player.md)
* [Profiling](profiling.md)
* [RenderDoc Integration](renderdoc.md)

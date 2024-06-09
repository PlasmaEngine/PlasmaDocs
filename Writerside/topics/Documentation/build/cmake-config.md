# CMake Setup

To generate a solution, run the CMake GUI. Specify *Where is the source code* and *Where to build the binaries*, then run **Configure**. As a generator, pick *Visual Studio 2022 x64* (or one of the other [supported platforms](supported-platforms.md)).

* **PLASMA_ENABLE_QT_SUPPORT** Disable this setting, if you want to compile Plasma without Qt. This will remove all editor code and several tools from the final solution. The default is *on*. When possible the Plasma CMake scripts will automatically download Qt libraries and set everything up for you. On configurations for which we do not support fully automatic setup, you need to install Qt manually and then set set **PLASMA_QT_DIR** to its installation folder.

* **PLASMA_BUILD_FMOD** Enable this, if you want to [FMOD sound](../sound/fmod-overview.md) support in your build. One Windows and Linux the default is *on*.

* **PLASMA_BUILD_PHYSX** Enable this, if you want to add [NVIDIA PhysX](../physics/physx/physx-overview.md) support to your build. Once enabled, the next run of "Configure" will automatically download PhysX binaries (Windows only) and set the **PLASMA_PHYSX_SDK** variable accordingly. The default is *off*. Note that PhysX support has been superseded by the [Jolt Physics integration](../physics/jolt/jolt-overview.md).

* **PLASMA_BUILD_RMLUI** Enable this, if you want to add support for [RmlUi](https://github.com/mikke89/RmlUi) to your build. The default is *on*.

Once you have configured everything, run **Generate** and then **Open Project**.

## Adding a Custom Project

The easiest way to get started with a custom project, is to use the [C++ project generation](../custom-code/cpp/cpp-project-generation.md).

Another method is to copy an existing sample, such as the [Sample Game Plugin](../../samples/sample-game-plugin.md). For starters, just create it in the same location, within the Plasma source tree. If you want to move it into your own repository, you can then reference its location as an *external project* (see below).

## External Projects

The options **PLASMA_EXTERNAL_PROJECT_1-3** allow you to specify folders outside the Plasma repository, which will be integrated into the solution. This is the most practical way to store your own code in a separate repository, yet have it all compiled in the same solution. This makes building, linking and debugging code as convenient as if it was stored inside the Plasma file structure.

## Build Filter

The option **PLASMA_BUILD_FILTER** allows you to strip down the code that is included in the solution. This is mainly meant for use cases where Plasma is [integrated as a submodule](submodule.md) and you only need parts of its functionality.

## Advanced CMake Options

Checking *Advanced* in the CMake GUI will show additional options to configure the Plasma build. These are mostly used to remove specific 3rd party code (and all dependent features). This is particularly helpful, if you want to buildPlasmaon a platform on which one of the dependencies may not compile.

## See Also

* [Supported Platforms](supported-platforms.md)
* [C++ Project Generation](../custom-code/cpp/cpp-project-generation.md)
* [PlasmaEngine as a Submodule](submodule.md)

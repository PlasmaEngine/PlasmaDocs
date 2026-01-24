# Build

This article describes how you can build the engine yourself, which enables you to extend the engine with custom functionality.

## Platform Builds

* [Windows Builds](build-windows.md)
* [UWP Builds](build-uwp.md)
* [Linux Builds](build-linux.md)
* [MacOS Builds](build-macos.md)
* [Android Builds](build-android.md)
* [Building with Clang on Windows](clang-on-windows.md)

## Build Types

PLASMA sets up three build configuration types:

1. **Debug**
2. **Dev**
3. **Shipping**

While developing your game you should either use a **Debug** or a **Dev** build.

The **Debug** build is best when you want to use a C++ debugger to investigate problems. It includes the necessary *debug symbols* and has many optimizations disabled, which makes it much easier to step through the code. Debug builds are significantly slower than the other build types.

The **Dev** build has most of the optimizations enabled, yet still includes *debug symbols*. The *Dev* build is 3x to 10x faster than a *Debug* build in most cases and is very close to the speed of a *Shipping* build. Stepping through the C++ code with a debugger is possible, though it often behaves erratic due to the optimizations (inlining and such). For most developers the *Dev* build should be the main configuration to use.

The **Shipping** build has all optimizations enabled. It does not include *debug symbols* anymore and it also has all the developer features disabled. That means things like [plInspector](inspector.md) won't work here. Similarly, features like *allocation tracking* (for detecting memory leaks) and [profiling features](profiling.md) are disabled as well.

## See Also

* [Supported Platforms](supported-platforms.md)
* [Plasma Engine as a Submodule](submodule.md)

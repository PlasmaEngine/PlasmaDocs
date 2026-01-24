# Building Plasma

This article is designed to provide information on building Plasma. It will cover the high level of the build process and important concepts.

## Build Platforms

Plasma supports multiple build platforms, including:
- Linux (WIP)
- MacOS (Currently no rendering)
- [Windows](Building-For-Windows.md)
- Android (WIP)

Each platform has its own set of requirements and build instructions.

## Vulkan
The engine do not depend on the Vulkan SDK. All required dependencies are handled stored within the third party folder.
As a result the Vulkan SDK is now optional if you require the following features:
- Vulkan Debugging via validation layers
- Access Vulkan development tools.

The Vulkan loader is dynamically loaded at runtime, so Plasma will work on systems with or without Vulkan installed.

>**Note for C++ Developers:** </br>
> Direct Vulkan C function calls are not supported and will cause linker errors. You must use Vulkan-hpp (C++ wrapper) functions instead. The vulkan.hpp header is only included in RendererVulkanDLL.h with the appropriate defines configured.
{style="note"}

## Build Types
Plasma sets up three build configurations:
1. Debug
2. Dev
3. Shipping

While developing your game you should either use a Debug or a Dev build.

The Debug build is best when you want to use a C++ debugger to investigate problems. It includes the necessary debug symbols and has many optimizations disabled, which makes it much easier to step through the code. Debug builds are significantly slower than the other build types.

The Dev build has most of the optimizations enabled, yet still includes debug symbols. The Dev build is 3x to 10x faster than a Debug build in most cases and is very close to the speed of a Shipping build. Stepping through the C++ code with a debugger is possible, though it often behaves erratic due to the optimizations (inlining and such). For most developers the Dev build should be the main configuration to use.

The Shipping build has all optimizations enabled. It does not include debug symbols anymore and it also has all the developer features disabled. That means things like Inspector won't work here. Similarly, features like allocation tracking (for detecting memory leaks) and profiling features are disabled as well.

## Static Linking
On some platforms, such as Android, all code needs to be statically linked. In this case some of the automatisms used to load and configure the engine may not work correctly, because the linker optimizes away code that it deems unreferenced.

## See Also
- [Inspector](inspector.md)

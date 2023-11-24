# Plasma Engine as a Submodule

When using git and CMake for a project, Plasma Engine can be integrated as a submodule into the git repository and referenced from CMake.

First PlasmaEngine needs to be added as a submodule to git:

```cmd
git submodule add https://github.com/PlasmaEngine/PlasmaEngine.git
```

Additionally, if you want to use the precompiled tools and the sample content from Plasma, you also need to pull in its submodules as well:

```cmd
cd PlasmaEngine
git submodule init
git submodule update
```

Next, add the Plasma Engine folder in your root `CMakeLists.txt`:

```cmake
# Set the build filter, if you only want to integrate parts of Plasma into your build.
# set(PLASMA_BUILD_FILTER "FoundationOnly")

add_subdirectory(PlasmaEngine)
```

The Plasma Engine language detection can be reused by including the Plasma Engine submodule utility file:

```cmake
# include the Plasma submodule utility CMake functions
include("PlasmaEngine/Code/BuildSystem/CMake/plUtilsSubmodule.cmake")

pl_detect_languages()

project("MyProject" LANGUAGES ${PLASMA_LANGUAGES})
```

> **Important:**
>
> This kind of integration is useful, if you want to integrate Plasma *code* into your project, for instance, if you want to use plFoundation as your base library. Since the Plasma folder isn't top-level in this setup, using the full engine and all the data located in the [data directories](../projects/data-directories.md) won't work out of the box. For additional options, see the [CMake setup](cmake-config.md) page.

## Strip Unnecessary Code

When integrating Plasma this way, you may only want a subset of the available functionality. For instance, you may only need the plFoundation base library (and 3rd party dependencies). You can achieve this by configuring the [build filter](cmake-config.md#build-filter)

## SDK Root Folder

When integrating Plasma as a submodule, it is common for the binaries to be located outside of the Plasma Engine sub-folder, which means the engine won't be able to find the SDK root folder anymore. See [this article](sdk-root.md) for ways to fix this.

## See Also

* [CMake Setup](cmake-config.md)

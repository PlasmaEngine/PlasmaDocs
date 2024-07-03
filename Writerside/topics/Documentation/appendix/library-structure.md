# Library Structure

This document gives an overview of the functionality that Plasma Engine provides and how the most important libraries are structured.

Plasma Engine is divided into multiple libraries that provide different functionality.

The most basic and also largest library is **Foundation**. It contains all the basic functionality on which the rest of the engine is built. **Foundation** is meant to be application agnostic. All its features can be used in any kind of application. Most of the platform abstractions are implemented here.

Foundation itself only depends on various third-party libraries.

The **Core** library is built on top of Foundation. This library contains engine specific features, such as the Game Object system. **Core** is where most of the actual engine infrastructure is implemented.

**System** is the library that is supposed to contain all the high-level platform specific code that might be difficult to abstract. Currently this mostly contains window creation code.

The **TestFramework** library implements code to manage our unit-tests. You can ignore this entirely.

**GameEngine** builds on top of all the other libraries, including the rendering code. It contains the most high-level code for a game engine, such as AI and Animation, [plGameApplication (TODO)](../runtime/application/application.md) and [plGameState](../runtime/application/game-state.md), which are the basis for any game application built with Plasma, the prefab system, the visual scripting and much more.

In general the most interesting libraries to look at are **Foundation**, **Core** and **GameEngine**.

## Library Overview: Foundation

The Foundation library contains all the 'low-level' code that is used throughout the engine.

In **Foundation\\Containers** you will find different types of container classes. These are heavily influenced by the STL, so a lot might look familiar. The most interesting class one should have a look at is `plHybridArray`.

In **Foundation\\Strings** you will find all the string classes and utilities. Plasma Engine works with Utf-8 strings everywhere, which makes some things a bit more complicated, but these string classes make it pretty easy. There are utility classes to work with raw C strings and higher-level string classes to create and store strings efficiently.

In **Foundation\\Math** you will find lots of math classes, e.g. classes to do vector arithmetic (`plVec3`, `plMat4`, `plQuat`, `plPlane`, etc.), classes to work with colors (`plColor`, `plColorGammaUB`, `plColorLinear16f`), classes to work with bounding volumes (`plBoundingBox`, `plBoundingSphere`) and do culling (`plFrustum`), utility functions for intersection tests (`plIntersectionUtils`) and a class to work with angles efficiently (`plAngle`). There is even an implementation for a fixed point type (`plFixedPoint`).

In **Foundation\\Time** you will find `plTime`, which handles simple time values. Using `plTime::Now()` you can access the current application time. To handle game time (e.g. for slow-motion, etc.) use `plClock`. For profiling or timing `plStopwatch` is available. And finally for system-independent timestamps, which might be useful when working with file modification times, `plTimestamp` and `plDateTime` are provided.

In **Foundation\\Threading** you will find functionality that is useful for threading. `plAtomicInteger` provides lock-free integer values. `plLock` and `plMutex` implement the standard mechanisms for working with critical sections. `plThread` is a platform independent implementation for threads and `plThreadSignal` allows to send signals to other threads. `plThreadUtils` provides some of the low-level threading functions, such as `plThreadUtils::Sleep()`.
However, before you go ahead and create your own threads, you should have a look at `plTaskSystem`, which is a thread-pool implementation that efficiently distributes tasks across multiple worker threads. It supports dependencies across tasks, different priorities, waiting/blocking for unfinished tasks, task canceling and load-balancing when tasks run over multiple frames. There should be only very few situations where a task is not good enough and a custom thread is necessary.

In **Foundation\\Logging** you will find `plLog`, the central class to output log information. There are various ways logging information can be output. `plLogWriter::HTML` allows to write the data to an HTML file, `plLogWriter::Console` and `plLogWriter::VisualStudio` output the data to different console windows. Additionally the [plInspector](../tools/inspector.md) tool will display all logged data as well. The logging system is extremely useful to get an insight into what your application is doing and what might be going wrong, so we suggest setting this up early and using it to log most of what your application is doing.

In **Foundation\\Algorithm** you will find some useful algorithms, mostly for sorting, searching and hashing.

In **Foundation\\Basics** you can find a lot of platform specific code, most of which might not be very interesting. You will also find `PL_ASSERT` which you should be using frequently.

In **Foundation\\Basics\\Types** you will find some fundamental types that are used frequently in Plasma. `plDelegate` is often used for callbacks. `plEnum` is used for type-safe enum types and `plBitflags` is used for type-safe and easy to use bitflags. `plArrayPtr` is a 'fat pointer' that stores the start and length of an array. Finally `plVariant` is a type that can store different types of data (float, int, string, vector, etc.) and knows which type it has stored. It can do conversions between related types and is often used in message passing.

In **Foundation\\CodeUtils** you can find utilities to work with code or text, such as `plTokenizer`. You will also find a full implementation of a C preprocessor (`plPreprocessor`).

In **Foundation\\Communication** you can find functionality to communicate with other code. `plEvent` is a frequently used class to raise events and thus inform other code of changes. `plMessage` is used for message passing, which is quite often used with the game object system (which you will find in the **Core** library). `plTelemetry` is a system to broadcast information from the running application to other applications, usually tools for introspection, such as [plInspector](../tools/inspector.md).

In **Foundation\\Configuration** you will find tools to configure the application. `plStartup` is a system to (de-)initialize different subsystems in your code in the right order. `plPlugin` is used when you want to extend your application using plugin DLLs dynamically at runtime. `plStartup` helps with this as well.
`plCVar` is a 'configuration variable' that allows to easily change the state of the running application. Its state can be stored on disk and it can be modified either through an `plConsole` or remotely through plInspector. This allows to have lots of 'debug modes' that can be enabled on demand without recompilation or complicated integration into the input handling.

In **Foundation\\Utilities** you will find some utility functionality, such as `plCommandLineUtils` for command-line argument parsing, `plConversionUtils` for string / number conversions and `plStats` for broadcasting the state of some internal code, which is useful for debugging game code.

In **Foundation\\IO** you will find lots of functionality for reading and writing data.

`plStreamReader` and `plStreamWriter` are the interfaces for all IO operations. Derived from these classes you will find `plMemoryStreamReader` / `plMemoryStreamWriter` for working with data in-memory. `plCompressedStreamReaderZstd` and `plCompressedStreamWriterZstd` allow to zip and unzip data and `plChunkStreamWriter` / `plChunkStreamReader` implement a 'chunked' format that can be used for building file formats that another application may not fully understand.

`plOSFile` is the low-level file abstraction, in most cases you should not need to work with this. Instead prefer [plFileSystem](../runtime/filesystem.md) which adds functionality for virtual file systems through mount points. For example a compressed file or a remote folder may be mounted as a read-only directory. `plFileSystem` is the central class to manage file accesses, but to actually read or write a file, use `plFileReader` and `plFileWriter`, which also implement the `plStream*` interface.

To store data in a structured way, `plJSONWriter` and `plOpenDdlWriter` are provided. For convenient retrieval `plJSONReader` and `plOpenDdlReader` are available. For less convenient but more flexible and efficient JSON/[OpenDDL](http://openddl.org/) reading you can also use `plJSONParser` or `plOpenDdlParser`.

In **Foundation\\Reflection** you will find the reflection system of Plasma Engine. This is used by the game objects and some other high-level code for object type identification and properties. This may be used for scripting, for setting up objects from configuration files and for editors. Most notable classes are `plRTTI` and `plReflectedClass`.

## Library Overview: Core

In **Core** you will find the core engine infrastructure.

In **Core\\Application** you can find code to more easily set up your application loop in a platform independent way.

In **Core\\Graphics** you will find code commonly needed for doing graphics, such as `plCamera` for camera controls and `plGeometry` to create geometric objects.

In **Core\\Input** you will find `plInputManager` which can be used for retrieving input from various different devices, e.g. mouse, keyboard, gamepad or virtual thumbstick. The system is easily extensible to include custom devices.

In **Core\\ResourceManager** you will find the static class `plResourceManager` which is the central class for resource loading (e.g. textures, shaders, etc.). For implementing custom resource types you need to derive from `plResource` and for customizing the loading procedure you may need to implement a custom `plResourceTypeLoader`. All resources are referenced through `plResourceHandle` types, which implement reference counting.

In **Core\\Scripting** you can find `plLuaWrapper` that allows to easily work with Lua scripts.

In **Core\\World** you will find the game object system. `plGameObject` is the class to use to manage entities, `plComponent` is the base component class that allows to implement and attach components to your entities. All entities belong to an instance of `plWorld`, which represents your scene graph.

## Library Overview: GameEngine

In **GameEngine** you will find all the high-level code needed in a game engine.

**GameEngine\\Console** contains code for a Quake-like in-game console that can be used for changing the game configuration (through `plCVar` or custom functions) and to see the `plLog` output.

**GameEngine\\GameApplication** contains [plGameApplication (TODO)](../runtime/application/application.md), which extends `plApplication` with higher-level, more game specific functionality. This is one of the most important high-level classes to look at and extend when writing your own, stand-alone game application (assuming you can't do so with `plGameState` alone).

In **GameEngine\\GameState** you find [plGameState](../runtime/application/game-state.md), which is the most important class to extend when writing your own game code, especially if you want to be able to run your code within the editor.

**GameEngine\\Interfaces** contains various interface definitions for instance for basic interactions with physics and audio engines.

**GameEngine\\Prefabs** contains the code to work with prefabs.

## Library Overview: Texture

In **Texture** you will find various things related to working with images and textures.

In **Texture\\Image** you will find `plImage` which can be used to read, write and convert images from various formats.

## Library Overview: Utilities

In **Utilities** you will find various different things that may be useful, but are not used by the general engine runtime. They may be used by some tool or by a sample game, though.

**Utilities\\DataStructures** contains data structures that are too engine specific. Here you will find things such as octree and quadtree implementations (`plDynamicOctree`).

**Utilities\\GridAlgorithms** contains functionality to rasterize circles and lines into grids. This can be extremely useful for 2D top down games, like strategy games, to do line-of-sight computations and such.

**Utilities\\PathFinding** contains functionality to do path searches on graphs and simple nav-mesh generation for 2D grids.

## See Also


* [Samples](../../samples/samples-overview.md)

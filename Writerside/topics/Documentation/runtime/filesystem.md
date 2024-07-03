# FileSystem

Accessing files is one of those things that you probably need to do very early in your project. Although the POSIX functions fopen, fread, etc. are available on most platforms, they are not always the best choice. PlasmaEngine provides multiple layers of abstractions for accessing files, or more generally, data streams that look like files.

## Overview

The following is a list of abstractions that you should be aware of. Each one will be explained in more detail below.

* __Streams__ (`plStreamReader`, `plStreamWriter`) are the basis for all reading and writing of abstract data streams. These are the two classes that you will use whenever something that acts like a file is passed around, even though it does not need to represent an actual file.
* __Low Level File Abstraction__ (`plOSFile`): This is the abstraction layer that implements reading and writing to actual files on disk in a mostly platform independent manner. This is what you typically should not need to use, at all. However, when something is not possible through the higher level abstractions, you might need to do it through this interface.
* __High Level File System__ (`plFileSystem`, `plFileReader`, `plFileWriter`): Through `plFileSystem` you can configure a virtual file-system. `plFileReader` and `plFileWriter` should be what you typically use to open 'files' in that virtual file-system. `plFileReader` and `plFileWriter` implement the respective stream interfaces `plStreamReader` and `plStreamWriter`, so once you have opened a file through these classes, you can pass them to any function that works on streams.

## Streams

A 'stream' is simply a series of bytes. This data stream can come from a physical file, through a network or it can be generated fully procedurally.

Streams typically come in two forms: Ones that you can read from and ones that you can write to. In PlasmaEngine those two types of streams are represented with the interface classes `plStreamReader` and `plStreamWriter` respectively. The stream interfaces are reduced in functionality to what all types of data streams can provide. Reading is always done from the current read position. Writing will always append data at the end of the stream. You cannot seek to an arbitrary position (when reading you can skip ahead) and you cannot re-read the same data or overwrite previously written data.
Although this can be limiting in a few scenarios, it is absolutely sufficient for the vast majority of use cases. For the few cases where you really need to set the read or write position, you can revert to another abstraction layer, e.g. on an `plOSFile` you have more control.
  
Inside the core engine we typically do not care about files, at all. Therefore you will not find many functions that take a file-name string. In the few cases that this is so, those functions are usually just convenience functions that internally open a file and then pass along the file as a stream.
Instead most engine functions work directly on streams. This decouples the engine from working on the concept of files and enables to work on data from any kind of source. For example, this makes it easy to embed a file in an archive or to read it from a network, or even both combined.

### Memory Streams

A very frequently used implementation of streams is the 'memory stream'. This represents a stream of data that exists in RAM only. The data is stored in an `plMemoryStreamStorage` object. You can have multiple readers through the `plMemoryStreamReader` class and you could theoretically have multiple writers through the `plMemoryStreamWriter` class (though having more than one will probably not work in any useful way).

Plasma Engine often uses memory streams to store incoming data for fast access later. For example the `plResourceManager` reads files from disk on a separate thread into a memory stream. This allows to do the slow file reading in parallel without blocking the main thread. Once all data is read into the memory stream, the main thread can then read the data directly from memory and have a guaranteed latency. The interface for reading from file or the memory stream is identical, so the code that actually interprets the file content does not need to know about this optimization at all.

### Other Types of Streams

Plasma Engine comes with a variety of stream implementations:

* __Compressed Streams__: Through `plCompressedStreamReaderZstd` and `plCompressedStreamWriterZstd` you can easily add compression to your data streams. These classes take another stream as input or output, so you can pass it a file or memory stream to work upon.
* __Chunk Streams__: A chunk stream is basically a stream that is divided into distinct parts which are fully separated from each other. This allows to handle one stream (e.g. a file) as if it were actually multiple streams, which is useful when you want to package multiple files into one. The useful feature of these streams is that code often reads a stream until it ends (e.g. nothing more can be read). When you package multiple files into one stream, this behavior can end badly. A chunk stream enables you to prevent code from reading further than a specific point (a virtual 'end-of-stream' position).
Chunk formats are also useful when you only want to read or update certain parts of a file, without knowing how the rest of the file format works. This is possible because the size of each chunk is stored in the stream which allows to skip or read an entire chunk and pass it through.
  
Please note that you can combine different types of streams. For example you can write to a file by using `plFileWriter`, pass that stream to `plChunkStreamWriter` and then even use `plCompressedStreamWriterZstd` to compress individual chunks in the file.

### Using Standard Types with Streams

The stream interfaces only provide the functions `ReadBytes` and `WriteBytes`. For most standard types Plasma Engine provides overloaded `<<` and `>>` operators. E.g. you can read and write `ints`, `floats`, `plVec3`, `plString`, etc. like this:

```cpp
write_stream << plVec3(1, 2, 3);
write_stream << "some string";

plVec3 v;
plString s;
read_stream >> v;
read_stream >> s;
```

### Using Complex Types with Streams

To serialize and deserialize data that is in Plasma containers, you can also use functions like `plStreamReader::ReadArray()`, `plStreamReader::ReadMap()`, `plStreamWriter::WriteArray()` and `plStreamWriter::WriteMap()`. Those functions will try to serialize the container information and all the elements. For that to work, there must either be `<<` and `>>` operaters overloaded for the element type, or the element types must have member functions with the following signature:

```cpp
plResult Serialize(plStreamWriter& stream) const;
plResult Deserialize(plStreamReader& stream);
```

Using these functions allows to return success or failure, which is not possible with the shift operators. If any element fails to de-/serialize, the whole operation (e.g. `plStreamWriter::WriteArray()`) will fail and terminate early.

**Note:** `plStreamWriter::WriteArray()` and similar functions are provided for convenience. However, when it is important to have full control over file versioning and backwards compatibility of a file format, it may be preferable to serialize containers manually.
  
## Low Level File Abstraction

Reading and writing files is implemented through `plOSFile`. This class internally uses platform specific functions such as `fopen` on Linux and `CreateFile` on Windows. You should typically NOT use this class, there are higher level abstractions built upon `plOSFile` that you should prefer.

Since `plOSFile` provides actual file access, it also has some file specific features, for instance you can set the file read or write position back and forth and you can get the OS specific file handle, such that you can use OS specific functions on that file yourself.

Additionally there are static functions for deleting files, creating directory structures, querying whether a file exists, and so on.

`plOSFile` is a thin abstraction over the operating system, it does not yet implement a higher level interface. Therefore it deliberately does not implement the stream interfaces, so you cannot pass an `plOSFile` instance to a function that takes an `plStreamReader` or `plStreamWriter`.

Usually you only need to use `plOSFile` for some of the static functions that implement more infrequently used features, such as `plOSFile::CopyFile` or `plOSFile::GetFileStats`. These might not be available in higher level abstractions.

Please be aware that `plOSFile` always requires platform specific absolute paths. There is no concept of a 'current working directory' or some root directory, to which relative paths could be used. `plOSFile` will check all incoming paths and assert that they are absolute. Therefore, if you need to use `plOSFile`, make sure to always convert any relative path to an absolute path before you pass it to `plOSFile`.

### Other Low Level File Operations

Apart from `plOSFile`, there are a few classes that implement additional file system operations that are only thin abstractions over the operating system.

**plFileSystemIterator** is a class that allows to iterate over all files and folders in some directory. In a game this should rarely be necessary, but in tools this can be very useful. Unfortunately it is not guaranteed that this feature can be implemented on all platforms, and each platform might have different features regarding wild-card usage and so on. Therefore this class is only available when the preprocessor define `PL_SUPPORTS_FILE_ITERATORS` is defined as `PL_ON`.

**plFileStats** is a struct that provides information about a file or folder. One way to retrieve file stats is through `plOSFile::GetFileStats()`. Again, this feature cannot be implemented on all platforms, so it is only available when `PL_SUPPORTS_FILE_STATS` is defined as `PL_ON`.

## High Level File System

Plasma Engine comes with a high level file system that is very flexible and powerful but might seem a bit confusing at first for people that are not used to working with abstractions on this level.

A game engine is in many aspects simply a framework that manages resources. It ensures that resources can be found and accessed, are freed when not needed any more and otherwise are handled efficiently and often in an abstract manner that makes it easy to work with them.

Working with files and everything that is similar enough so that it could be handled like a file, is the lowest level at which this 'managing of resources' begins.

Plasma Engine does this by working with a virtual file system. The central class to configure this file system is `plFileSystem`.

### Data Directories

The most important concept that you need to understand is that of 'data directories'. A data directory is basically a mount point that is added to the virtual file system. You can have an arbitrary number of those, but usually you will only need very few.

A data directory is in the most common use case some folder on your harddisk. By adding it to the file system (using `plFileSystem::AddDataDirectory`) you make that folder visible for the application.

When you work with the virtual file system, you do NOT use `plOSFile`. Instead, you will most likely use `plFileReader` and `plFileWriter`. Those classes represent a single open file in the virtual file system. They implement the stream interfaces mentioned above.

When you open a file through these classes, you should use relative paths. Absolute paths will only work if a data directory above the given path is also mounted. When you open a file through a relative path, all data directories are searched (in the reverse order in which they were added) for the file. So as long as the file exists in one data directory, it can be opened. If it exists in multiple data directories with the same relative path, you will typically get the file from the data directory that was added last.

The use case here is, that you often want to have some 'base' data directory that contains general files and than additional data directories that add project or even level specific files to the file system. You will typically add the 'base' data directory right at startup of your game. Later you add your project specific data directories. Since you often want your files in the project data directory to take precedence over the 'base' data directory, it makes sense for the file system to search the directories in the reverse order in which they were added.

One use case for multiple data directories with the same files in it is localization. Suppose you have a folder with all your sounds, including speech that is recorded in English. When you want to add another language, you can just create a folder 'German' that only contains the sound files which need localization. When the user wants German language support, you simply mount the German sounds folder AFTER the other data directory. Now whenever a sound file gets loaded that is both in the German sounds data directory and the default data directory, the German sound will be preferred. Everything that is not there falls back to the default data directory. Thus when some sound file was forgotten to be included in the German localization, the game will at least play the sound in English.

### Advanced Data Directories

Although the most common use case is to mount folders as data directories, Plasma Engine's concept of data directories goes much further. Basically anything can be 'mounted' as a data directory. For example you could mount a zip file and then use it like a read-only folder. Or you could mount a folder on a remote PC and have the data sent over a network.

This is possible because data directories are an abstract concept. To create your own type of data directory, you need to implement three classes, derived from `plDataDirectoryType`, `plDataDirectoryReader` and `plDataDirectoryWriter` respectively.

Therefore, when you add a data directory to `plFileSystem`, the engine needs to know how exactly to mount this type. This is what 'data directory factories' are necessary for. So for example, if you want to support simple folders and zip files as data directories, you need to register one factory for 'folders' and one factory for 'zip archives'.
Now when you mount a data directory with the name "My/Test/Archive.zip", the engine will ask each factory, whether it can handle this path. The 'folder factory' will detect that this is a file and not a folder and therefore decline. The 'zip factory' detects that this is a zip file and therefore creates a data directory which provides the functionality to read files from the archive as if it were a real folder. For example you could then open a file with the path "My/Test/Archive.zip/Some/Compressed/File.txt" through `plFileReader` and it would just work as if the file was located in a real folder.

That is why you always need to register these factories first, before you can add any data directories to the virtual file system.

If you want to implement your own data directory type, please have a look at `plDataDirectory::FolderType`.

### Setting up the File System

Setting up the file system is very easy to do, once you know what is involved and why. The most basic configuration looks like this:

```cpp
// register a factory that can handle simple folders
// this is actually already done automatically through the plStartup system
// plFileSystem::RegisterDataDirectoryFactory(plDataDirectory::FolderType::Factory);

// mount the application directory (where the binary is located) as a data directory
plFileSystem::AddDataDirectory(plOSFile::GetApplicationDirectory());
```

That's all.

Now you can read and write files in that folder like this:

```cpp
plFileWriter FileOut;
if (FileOut.Open("SubFolder/Test.txt") == PL_SUCCESS)
{
    // "SubFolder" will be created automatically, if it does not exist yet

    FileOut << "This is a string";
    FileOut.Close(); // will also be called automatically when FileOut goes out of scope
}

plFileReader FileIn;
if (FileIn.Open("SubFolder/Test.txt") == PL_SUCCESS)
{
    plString s;
    FileIn >> s;
    FileIn.Close(); // will also be called automatically when FileIn goes out of scope

    PL_ASSERT_DEV(s == "This is a string", "The read string is incorrect: '%s'", s.GetData());
}
```

Obviously you can now add further data directories through `plFileSystem::AddDataDirectory()`. There are several additional features to configure the system for your exact use case. Please have a look at the API documentation for further details.

### Resolving Paths

One thing that comes up once in a while is that you need to convert a path from relative to absolute or vice versa.

For example, should you actually need to use an `plOSFile` function and therefore you require the absolute path to a file, of which you only know the relative path (in some data directory), you need a way to query this information.

This is what `plFileSystem::ResolvePath()` is for.

Basically you give it some path, and it will return under which absolute path and under which relative path the file was found. It also needs to know whether you want to read or write the file. If you want to read it, ie. the file is supposed to already exist, it will search for the file in all data directories. If you want to write it, it will return under which path the file would end up.

## See Also



 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddTrailingDirectorySeparator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#addtrailingdirectorysepa)|[ DirectorySeparator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#directoryseparator-plasma)| | |
|[ ChangeExtension](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#changeextension-plasma-eng)|[ ExecutableDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#executabledirectory-plasma)| | |
|[ CombineDirectories](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#combinedirectories-plasma)|[ ExecutableFile](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#executablefile-plasma-engi)| | |
|[ CombineDirectoriesAndFile](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#combinedirectoriesandfil)|[ TemporaryDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#temporarydirectory-plasma)| | |
|[ GetCanonicalizedPathFromAbsolutePath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getcanonicalizedpathfrom)|[ UserDocumentsDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#userdocumentsdirectory-z)| | |
|[ GetComparablePathFromAbsolutePath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getcomparablepathfromabs)|[ UserLocalDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#userlocaldirectory-plasma)| | |
|[ GetDirectoryName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getdirectoryname-plasma-en)|[ WorkingDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#workingdirectory-plasma-en)| | |
|[ GetDirectoryPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getdirectorypath-plasma-en)| | | |
|[ GetExtensionWithDot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getextensionwithdot-plasma)| | | |
|[ GetExtensionWithoutDot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getextensionwithoutdot-z)| | | |
|[ GetFileNameWithExtension](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getfilenamewithextension)| | | |
|[ GetFileNameWithoutExtension](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#getfilenamewithoutextens)| | | |
|[ IsRelative](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#isrelative-plasma-engine-d)| | | |
|[ RemoveTrailingDirectorySeparator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filepath.md#removetrailingdirectorys)| | | |


 #  Properties


---  
 #  DirectorySeparator : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> Gets the character(s) used for separating directories and files. This value is often different depending on the operating system (generally either '/' or '\')

> ``` lang=cpp, name=Lightning
> var DirectorySeparator : String


---  
 #  ExecutableDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> The directory the executable lives with in (exe, elf...). This will always include a directory separator at the end of the result.

> ``` lang=cpp, name=Lightning
> var ExecutableDirectory : String


---  
 #  ExecutableFile : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> A path directly to the executable itself (exe, elf...).

> ``` lang=cpp, name=Lightning
> var ExecutableFile : String


---  
 #  TemporaryDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> Temporary files should be placed here. This will always include a directory separator at the end of the result.

> ``` lang=cpp, name=Lightning
> var TemporaryDirectory : String


---  
 #  UserDocumentsDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> User saved data that the user can backup or modify should be placed here (read/write/create permissions should be allowed). This will always include a directory separator at the end of the result.

> ``` lang=cpp, name=Lightning
> var UserDocumentsDirectory : String


---  
 #  UserLocalDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only` `static`

> Application saved information should be placed here (read/write/create permissions should be allowed). This will always include a directory separator at the end of the result.

> ``` lang=cpp, name=Lightning
> var UserLocalDirectory : String


---  
 #  WorkingDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> A directory that all relative paths start resolving from. In general the changing of the working directory is discouraged because it may affect assumptions of the host application. This will always include a directory separator at the end of the result.

> ``` lang=cpp, name=Lightning
> var WorkingDirectory : String


---  
 #  Methods


---  
 #  AddTrailingDirectorySeparator : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Pass in a directory path with or without the separator and this will add it at the end (if needed).
Example: ('Content\Powerups') results in 'Content\Powerups\'
Example: ('Content\Powerups\') results in 'Content\Powerups\'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function AddTrailingDirectorySeparator(p0 : String) : String
> ``` 


---  
 #  ChangeExtension : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Changes the extension of a path (with file name at the end) to a new extension. If the file has no extension, then this will automatically add the extension to the end. The extension is allowed to contain a leading dot '.' character (or not). The path is also allowed to contain a trailing dot '.' character (or not).
Example: ('Content\Player.png', 'jpg') results in 'Content\Player.jpg'
Example: ('Content\Player', 'jpg') results in 'Content\Player.jpg'
Example: ('Content\Player.', '.jpg') results in 'Content\Player.jpg'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |p1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function ChangeExtension(p0 : String, p1 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectories(dir0 : String, dir1 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir2|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir2|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir3|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String, dir3 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir2|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir3|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir4|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String, dir3 : String, dir4 : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |fileName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectoriesAndFile(dir0 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |fileName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir2|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |fileName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, dir2 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir2|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |dir3|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |fileName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, dir2 : String, dir3 : String, fileName : String) : String
> ``` 


---  
 #  GetCanonicalizedPathFromAbsolutePath : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Changes all directory separators to be the current operating system directory separator, removes duplicate separators, and removes '..' and '.' from the paths. Canonicalized is only guaranteed to work on absolute paths. This behavior is operating system dependent and may call the related OS functions.
Example: ('C:/Sandbox//Engine/../Content/./Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetCanonicalizedPathFromAbsolutePath(p0 : String) : String
> ``` 


---  
 #  GetComparablePathFromAbsolutePath : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> First this normalizes the path, then if the operating system is case insensative, it will make the path all lowercase so that it compares.
Example: ('C:\Sandbox\Engine\..\Content\.\Player.png') results in 'c:\sandbox\content\player.png'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetComparablePathFromAbsolutePath(p0 : String) : String
> ``` 


---  
 #  GetDirectoryName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> If a file path is passed in, this will return the name of the parent directory. If a directory path is passed in (ending in a separator), this will return the name of the directory. A directory path without a trailing separator is abiguous with a file that has no extension. In this case, we always assume it is a file and therefore get the parent directory's name.
Example: ('Content\Powerups\Recharge.png') results in 'Powerups'
Example: ('Content\Powerups\') results in 'Powerups'
Example: ('Content\Powerups') results in 'Content'
Example: ('Content') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetDirectoryName(p0 : String) : String
> ``` 


---  
 #  GetDirectoryPath : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> If a file path is passed in, this will return the parent directory. If a directory path is passed in (ending in a separator), this will return the directy back with no modifications. A directory path without a trailing separator is abiguous with a file that has no extension. This will always include a directory separator at the end of the result. In this case, we always assume it is a file and therefore get the parent directory's name.
Example: ('Content\Powerups\Recharge.png') results in 'Content\Powerups\'
Example: ('Content\Powerups\') results in 'Content\Powerups\'
Example: ('Content\Powerups') results in 'Content\'
Example: ('Content') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetDirectoryPath(p0 : String) : String
> ``` 


---  
 #  GetExtensionWithDot : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Returns only the extension of a file (everything after the last dot, including the dot). If the file has no extension then this will return an empty string.
Example: ('Content\Player.png') results in '.png'
Example: ('Content\Player.') results in ''
Example: ('Parent.Directory\Log') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetExtensionWithDot(p0 : String) : String
> ``` 


---  
 #  GetExtensionWithoutDot : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Returns only the extension of a file (everything after the last dot, not including the dot). If the file has no extension then this will return an empty string.
Example: ('Content\Player.png') results in 'png'
Example: ('Content\Player.') results in ''
Example: ('Parent.Directory\Log') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetExtensionWithoutDot(p0 : String) : String
> ``` 


---  
 #  GetFileNameWithExtension : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Returns only the file portion of a path (everything past the last separator including the extension).
Example: ('Content\Player.png') results in 'Player.png'
Example: ('Content\Powerups\') results in ''
Example: ('Content\Powerups') results in 'Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetFileNameWithExtension(p0 : String) : String
> ``` 


---  
 #  GetFileNameWithoutExtension : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Returns only the file portion of a path (everything past the last separator excluding the extension).
Example: ('Content\Player.png') results in 'Player'
Example: ('Content\Powerups\') results in ''
Example: ('Content\Powerups') results in 'Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetFileNameWithoutExtension(p0 : String) : String
> ``` 


---  
 #  IsRelative : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `static`

> Returns true if a path has no root (such as a volume/hard drive specifier, or unix like systems a beginning slash). Even a beginning slash that means 'relative to the current working directory volume' is still relative. Empty paths will return that they are relative.
Example: ('C:\Sandbox\Engine\..\Content\.\Player.png') results in 'false'
Example: ('Sandbox') results in 'true'
Example: ('Content\Powerups\Recharge.png') results in 'true'
Example: ('/usr/Content/Player.png') results in 'false'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function IsRelative(p0 : String) : Boolean
> ``` 


---  
 #  RemoveTrailingDirectorySeparator : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Pass in a directory path with or without the separator and this will remove it from the end (if needed).
Example: ('Content\Powerups') results in 'Content\Powerups'
Example: ('Content\Powerups\') results in 'Content\Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveTrailingDirectorySeparator(p0 : String) : String
> ``` 


---  
 

 
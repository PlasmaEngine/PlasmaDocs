 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#clone-plasma-engine-docume)|[ Cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#cog-plasma-engine-document)|Object| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#cogpath-void)|[ DirectCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#directcog-plasma-engine-do)| | |
|[ ComputePath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#computepath-plasma-engine)|[ ErrorOnDirectLinkFail](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#errorondirectlinkfail-ze)| | |
|[ Refresh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#refresh-plasma-engine-docu)|[ ErrorOnPathCantCompute](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#erroronpathcantcompute-z)| | |
|[ RefreshIfNull](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#refreshifnull-plasma-engin)|[ ErrorOnResolveToNull](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#erroronresolvetonull-zer)| | |
|[ Resolve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#resolve-plasma-engine-docu)|[ Path](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#path-plasma-engine-documen)| | |
| |[ PathPreference0](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#pathpreference0-plasma-eng)| | |
| |[ PathPreference1](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#pathpreference1-plasma-eng)| | |
| |[ PathPreference2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#pathpreference2-plasma-eng)| | |
| |[ RelativeTo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#relativeto-plasma-engine-d)| | |
| |[ UpdateCogOnInitialize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#updatecogoninitialize-ze)| | |
| |[ UpdateCogOnPathChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#updatecogonpathchange-ze)| | |
| |[ UpdatePathOnCogChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md#updatepathoncogchange-ze)| | |


 #  Properties


---  
 #  Cog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Setting the cog manually may recompute the path if the option is set Getting the cog will attempt to resolve the cog if we don't already have one (or if the path options is set, it will always resolve)
> ``` lang=cpp, name=Lightning
> var Cog : Cog


---  
 #  DirectCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Setting the cog manually may recompute the path if the option is set Getting the cog will return whatever cog we already resolved, or null (it will not attempt to resolve)
> ``` lang=cpp, name=Lightning
> var DirectCog : Cog


---  
 #  ErrorOnDirectLinkFail : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is it an exception/notification if a direct link to the object cannot be resolved?
> ``` lang=cpp, name=Lightning
> var ErrorOnDirectLinkFail : Boolean


---  
 #  ErrorOnPathCantCompute : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is it an exception/notification if the path to an object cannot be computed?
> ``` lang=cpp, name=Lightning
> var ErrorOnPathCantCompute : Boolean


---  
 #  ErrorOnResolveToNull : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is an exception thrown if you try to access the Cog when it's invalid or not found?
> ``` lang=cpp, name=Lightning
> var ErrorOnResolveToNull : Boolean


---  
 #  Path : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Setting the path will invalidate the object until the next call to GetCog.
> ``` lang=cpp, name=Lightning
> var Path : String


---  
 #  PathPreference0 : [CogPathPreference](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference0 : CogPathPreference


---  
 #  PathPreference1 : [CogPathPreference](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference1 : CogPathPreference


---  
 #  PathPreference2 : [CogPathPreference](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference2 : CogPathPreference


---  
 #  RelativeTo : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> The cog that we compute paths relative to.
> ``` lang=cpp, name=Lightning
> var RelativeTo : Cog


---  
 #  UpdateCogOnInitialize : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether the cog path attempts to resolve an object when the object is fully initialized.
> ``` lang=cpp, name=Lightning
> var UpdateCogOnInitialize : Boolean


---  
 #  UpdateCogOnPathChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When we set the cog path, should we try and resolve the object (this also detects parse errors)
> ``` lang=cpp, name=Lightning
> var UpdateCogOnPathChange : Boolean


---  
 #  UpdatePathOnCogChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When we set the cog, should we try and recompute a path to the object?
> ``` lang=cpp, name=Lightning
> var UpdatePathOnCogChange : Boolean


---  
 #  Methods


---  
 #  Clone : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

> Creates a new copy of a cog path (since cog paths are reference counted and shared)
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : CogPath
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CogPath()
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)| |
> ``` lang=cpp, name=Lightning
> function CogPath( : CogPath)
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |path|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function CogPath(path : String)
> ``` 


---  
 #  ComputePath : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Computes a path from one object to another (or an absolute path if specified - 'from' can be null) If computing the path fails, this will return an empty string.
> |Name|Type|Description|
> |---|---|---|
> |from|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |to|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |pref|[CogPathPreference](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cogpathpreference)| |
> ``` lang=cpp, name=Lightning
> function ComputePath(from : Cog, to : Cog, pref : CogPathPreference) : String
> ``` 


---  
 #  Refresh : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Refresh() : Boolean
> ``` 


---  
 #  RefreshIfNull : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RefreshIfNull() : Boolean
> ``` 


---  
 #  Resolve : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `static`

> Resolves a cog from a path and a a relative object (or null for absolute paths) Returns null if it fails to find the cog, and will not throw an exception or assert.
> |Name|Type|Description|
> |---|---|---|
> |startFrom|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |path|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function Resolve(startFrom : Cog, path : String) : Cog
> ``` 


---  
 

 
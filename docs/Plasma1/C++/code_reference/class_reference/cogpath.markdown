 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#clone-plasma-engine-docume)|[ Cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#cog-plasma-engine-document)|Object| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#cogpath-void)|[ DirectCog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#directcog-plasma-engine-do)| | |
|[ ComputePath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#computepath-plasma-engine)|[ ErrorOnDirectLinkFail](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#errorondirectlinkfail-ze)| | |
|[ Refresh](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#refresh-plasma-engine-docu)|[ ErrorOnPathCantCompute](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#erroronpathcantcompute-z)| | |
|[ RefreshIfNull](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#refreshifnull-plasma-engin)|[ ErrorOnResolveToNull](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#erroronresolvetonull-zer)| | |
|[ Resolve](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#resolve-plasma-engine-docu)|[ Path](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#path-plasma-engine-documen)| | |
| |[ PathPreference0](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#pathpreference0-plasma-eng)| | |
| |[ PathPreference1](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#pathpreference1-plasma-eng)| | |
| |[ PathPreference2](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#pathpreference2-plasma-eng)| | |
| |[ RelativeTo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#relativeto-plasma-engine-d)| | |
| |[ UpdateCogOnInitialize](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#updatecogoninitialize-ze)| | |
| |[ UpdateCogOnPathChange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#updatecogonpathchange-ze)| | |
| |[ UpdatePathOnCogChange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown#updatepathoncogchange-ze)| | |


 #  Properties


---  
 #  Cog : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Setting the cog manually may recompute the path if the option is set Getting the cog will attempt to resolve the cog if we don't already have one (or if the path options is set, it will always resolve)
> ``` lang=cpp, name=Lightning
> var Cog : Cog


---  
 #  DirectCog : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Setting the cog manually may recompute the path if the option is set Getting the cog will return whatever cog we already resolved, or null (it will not attempt to resolve)
> ``` lang=cpp, name=Lightning
> var DirectCog : Cog


---  
 #  ErrorOnDirectLinkFail : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Is it an exception/notification if a direct link to the object cannot be resolved?
> ``` lang=cpp, name=Lightning
> var ErrorOnDirectLinkFail : Boolean


---  
 #  ErrorOnPathCantCompute : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Is it an exception/notification if the path to an object cannot be computed?
> ``` lang=cpp, name=Lightning
> var ErrorOnPathCantCompute : Boolean


---  
 #  ErrorOnResolveToNull : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Is an exception thrown if you try to access the Cog when it's invalid or not found?
> ``` lang=cpp, name=Lightning
> var ErrorOnResolveToNull : Boolean


---  
 #  Path : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> Setting the path will invalidate the object until the next call to GetCog.
> ``` lang=cpp, name=Lightning
> var Path : String


---  
 #  PathPreference0 : [CogPathPreference](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference0 : CogPathPreference


---  
 #  PathPreference1 : [CogPathPreference](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference1 : CogPathPreference


---  
 #  PathPreference2 : [CogPathPreference](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#cogpathpreference)

> 
> ``` lang=cpp, name=Lightning
> var PathPreference2 : CogPathPreference


---  
 #  RelativeTo : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> The cog that we compute paths relative to.
> ``` lang=cpp, name=Lightning
> var RelativeTo : Cog


---  
 #  UpdateCogOnInitialize : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Whether the cog path attempts to resolve an object when the object is fully initialized.
> ``` lang=cpp, name=Lightning
> var UpdateCogOnInitialize : Boolean


---  
 #  UpdateCogOnPathChange : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> When we set the cog path, should we try and resolve the object (this also detects parse errors)
> ``` lang=cpp, name=Lightning
> var UpdateCogOnPathChange : Boolean


---  
 #  UpdatePathOnCogChange : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> When we set the cog, should we try and recompute a path to the object?
> ``` lang=cpp, name=Lightning
> var UpdatePathOnCogChange : Boolean


---  
 #  Methods


---  
 #  Clone : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)

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
> ||[cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)| |
> ``` lang=cpp, name=Lightning
> function CogPath( : CogPath)
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |path|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function CogPath(path : String)
> ``` 


---  
 #  ComputePath : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

 `static`

> Computes a path from one object to another (or an absolute path if specified - 'from' can be null) If computing the path fails, this will return an empty string.
> |Name|Type|Description|
> |---|---|---|
> |from|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |to|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |pref|[CogPathPreference](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#cogpathpreference)| |
> ``` lang=cpp, name=Lightning
> function ComputePath(from : Cog, to : Cog, pref : CogPathPreference) : String
> ``` 


---  
 #  Refresh : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Refresh() : Boolean
> ``` 


---  
 #  RefreshIfNull : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RefreshIfNull() : Boolean
> ``` 


---  
 #  Resolve : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

 `static`

> Resolves a cog from a path and a a relative object (or null for absolute paths) Returns null if it fails to find the cog, and will not throw an exception or assert.
> |Name|Type|Description|
> |---|---|---|
> |startFrom|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |path|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Resolve(startFrom : Cog, path : String) : Cog
> ``` 


---  
 

 
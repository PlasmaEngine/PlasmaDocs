 `Engine`

(NOTE) A space is a near boundless, three-dimensional extent in which objects and events occur and have relative position, direction, and time. Essentially a world of objects that exist together. Used to divide objects between UI, World, Editor, and others. The two most Common spaces are the 'World' for the game world and the 'Ui' for the HUD and menus.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObjectsFromLevel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#addobjectsfromlevel-plasma)|[ AllObjects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#allobjects-plasma-engine-d)|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
|[ Create](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#create-plasma-engine-docum)|[ AllRootObjects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#allrootobjects-plasma-engi)| | |
|[ CreateAtPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#createatposition-plasma-en)|[ CurrentLevel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#currentlevel-plasma-engine)| | |
|[ CreateLink](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#createlink-plasma-engine-d)|[ IsEditorMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#iseditormode-plasma-engine)| | |
|[ DestroyAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#destroyall-void)|[ ObjectCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#objectcount-plasma-engine)| | |
|[ DestroyAllFromLevel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#destroyallfromlevel-void)| | | |
|[ FindAllObjectsByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findallobjectsbyname-zer)| | | |
|[ FindFirstObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findfirstobjectbyname-ze)| | | |
|[ FindFirstRootObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findfirstrootobjectbynam)| | | |
|[ FindLastObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findlastobjectbyname-zer)| | | |
|[ FindLastRootObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findlastrootobjectbyname)| | | |
|[ FindObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#findobjectbyname-plasma-en)| | | |
|[ GetModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#getmodified-plasma-engine)| | | |
|[ LoadLevel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#loadlevel-void)| | | |
|[ MarkModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#markmodified-void)| | | |
|[ MarkNotModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#marknotmodified-void)| | | |
|[ ReloadLevel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#reloadlevel-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md#space-void)| | | |


 #  Properties


---  
 #  AllObjects : [spacerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spacerange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllObjects : SpaceRange


---  
 #  AllRootObjects : [hierarchylistrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchylistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllRootObjects : HierarchyListRange


---  
 #  CurrentLevel : [level](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/level.md)

 `read-only`

> Last level loaded.
> ``` lang=cpp, name=Lightning
> var CurrentLevel : Level


---  
 #  IsEditorMode : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsEditorMode : Boolean


---  
 #  ObjectCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Number of objects in the space.
> ``` lang=cpp, name=Lightning
> var ObjectCount : Integer


---  
 #  Methods


---  
 #  AddObjectsFromLevel : [level](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/level.md)

> Add all objects from a level.
> |Name|Type|Description|
> |---|---|---|
> |levelName|[level](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/level.md)| |
> ``` lang=cpp, name=Lightning
> function AddObjectsFromLevel(levelName : Level) : Level
> ``` 


---  
 #  Create : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create an object in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function Create(archetype : Archetype) : Cog
> ``` 


---  
 #  CreateAtPosition : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a object at a position in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateAtPosition(archetype : Archetype, position : Real3) : Cog
> ``` 


---  
 #  CreateLink : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function CreateLink(archetype : Archetype, objectA : Cog, objectB : Cog) : Cog
> ``` 


---  
 #  DestroyAll : Void

> Destroy all objects in space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DestroyAll()
> ``` 


---  
 #  DestroyAllFromLevel : Void

> Destroy all objects created from level.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DestroyAllFromLevel()
> ``` 


---  
 #  FindAllObjectsByName : [cognamerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cognamerange.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindAllObjectsByName(name : String) : CogNameRange
> ``` 


---  
 #  FindFirstObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindFirstObjectByName(name : String) : Cog
> ``` 


---  
 #  FindFirstRootObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindFirstRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindLastObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastRootObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindLastRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindObjectByName(name : String) : Cog
> ``` 


---  
 #  GetModified : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetModified() : Boolean
> ``` 


---  
 #  LoadLevel : Void

> Load new level replace the current level.
> |Name|Type|Description|
> |---|---|---|
> |level|[level](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/level.md)| |
> ``` lang=cpp, name=Lightning
> function LoadLevel(level : Level)
> ``` 


---  
 #  MarkModified : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MarkModified()
> ``` 


---  
 #  MarkNotModified : Void

> Clears all modifications on this Cog. Does not clear LocalModificationOverride properties.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MarkNotModified()
> ``` 


---  
 #  ReloadLevel : Void

> Reload the current level.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReloadLevel()
> ``` 


---  
 #  Space : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Space()
> ``` 


---  
 

 
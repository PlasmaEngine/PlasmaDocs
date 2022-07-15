 `Engine`

(NOTE) A space is a near boundless, three-dimensional extent in which objects and events occur and have relative position, direction, and time. Essentially a world of objects that exist together. Used to divide objects between UI, World, Editor, and others. The two most Common spaces are the 'World' for the game world and the 'Ui' for the HUD and menus.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObjectsFromLevel](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#addobjectsfromlevel-plasma)|[ AllObjects](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#allobjects-plasma-engine-d)|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
|[ Create](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#create-plasma-engine-docum)|[ AllRootObjects](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#allrootobjects-plasma-engi)| | |
|[ CreateAtPosition](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#createatposition-plasma-en)|[ CurrentLevel](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#currentlevel-plasma-engine)| | |
|[ CreateLink](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#createlink-plasma-engine-d)|[ IsEditorMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#iseditormode-plasma-engine)| | |
|[ DestroyAll](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#destroyall-void)|[ ObjectCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#objectcount-plasma-engine)| | |
|[ DestroyAllFromLevel](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#destroyallfromlevel-void)| | | |
|[ FindAllObjectsByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findallobjectsbyname-zer)| | | |
|[ FindFirstObjectByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findfirstobjectbyname-ze)| | | |
|[ FindFirstRootObjectByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findfirstrootobjectbynam)| | | |
|[ FindLastObjectByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findlastobjectbyname-zer)| | | |
|[ FindLastRootObjectByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findlastrootobjectbyname)| | | |
|[ FindObjectByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#findobjectbyname-plasma-en)| | | |
|[ GetModified](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#getmodified-plasma-engine)| | | |
|[ LoadLevel](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#loadlevel-void)| | | |
|[ MarkModified](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#markmodified-void)| | | |
|[ MarkNotModified](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#marknotmodified-void)| | | |
|[ ReloadLevel](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#reloadlevel-void)| | | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/space.markdown#space-void)| | | |


 #  Properties


---  
 #  AllObjects : [spacerange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spacerange.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllObjects : SpaceRange


---  
 #  AllRootObjects : [hierarchylistrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/hierarchylistrange.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllRootObjects : HierarchyListRange


---  
 #  CurrentLevel : [level](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/level.markdown)

 `read-only`

> Last level loaded.
> ``` lang=cpp, name=Lightning
> var CurrentLevel : Level


---  
 #  IsEditorMode : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsEditorMode : Boolean


---  
 #  ObjectCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Number of objects in the space.
> ``` lang=cpp, name=Lightning
> var ObjectCount : Integer


---  
 #  Methods


---  
 #  AddObjectsFromLevel : [level](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/level.markdown)

> Add all objects from a level.
> |Name|Type|Description|
> |---|---|---|
> |levelName|[level](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/level.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddObjectsFromLevel(levelName : Level) : Level
> ``` 


---  
 #  Create : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create an object in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> ``` lang=cpp, name=Lightning
> function Create(archetype : Archetype) : Cog
> ``` 


---  
 #  CreateAtPosition : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a object at a position in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> |position|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateAtPosition(archetype : Archetype, position : Real3) : Cog
> ``` 


---  
 #  CreateLink : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
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
 #  FindAllObjectsByName : [cognamerange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cognamerange.markdown)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindAllObjectsByName(name : String) : CogNameRange
> ``` 


---  
 #  FindFirstObjectByName : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindFirstObjectByName(name : String) : Cog
> ``` 


---  
 #  FindFirstRootObjectByName : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindFirstRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastObjectByName : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindLastObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastRootObjectByName : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindLastRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindObjectByName : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindObjectByName(name : String) : Cog
> ``` 


---  
 #  GetModified : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

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
> |level|[level](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/level.markdown)| |
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
 

 
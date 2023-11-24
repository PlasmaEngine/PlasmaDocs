 `Engine`

(NOTE) Object cache is use to store objects at runtime.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearStore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#clearstore-void)|[ EntryCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#entrycount-plasma-engine-d)| | |
|[ Erase](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#erase-void)| | | |
|[ GetDirectoryPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#getdirectorypath-plasma-en)| | | |
|[ GetEntryAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#getentryat-plasma-engine-d)| | | |
|[ IsEntryStored](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#isentrystored-plasma-engin)| | | |
|[ IsStored](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#isstored-plasma-engine-doc)| | | |
|[ Restore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#restore-plasma-engine-docu)| | | |
|[ RestoreOrArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#restoreorarchetype-plasma)| | | |
|[ Store](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown#store-plasma-engine-docume)| | | |


 #  Properties


---  
 #  EntryCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Get number of entries in the ObjectStore.
> ``` lang=cpp, name=Lightning
> var EntryCount : Integer


---  
 #  Methods


---  
 #  ClearStore : Void

> Clear the store.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearStore()
> ``` 


---  
 #  Erase : Void

> Attempts to remove an object from the store.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Erase(name : String)
> ``` 


---  
 #  GetDirectoryPath : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> Returns the directory path to the object store.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetDirectoryPath() : String
> ``` 


---  
 #  GetEntryAt : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> Get the ObjectStore entry at the specified index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetEntryAt(index : Integer) : String
> ``` 


---  
 #  IsEntryStored : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Is there an entry record for the object in the store?
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsEntryStored(name : String) : Boolean
> ``` 


---  
 #  IsStored : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsStored( : String) : Boolean
> ``` 


---  
 #  Restore : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> Restore an object to the space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |space|[space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.markdown)| |
> ``` lang=cpp, name=Lightning
> function Restore(name : String, space : Space) : Cog
> ``` 


---  
 #  RestoreOrArchetype : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> Restore an object if it is not stored use the archetype to create it.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.markdown)| |
> |space|[space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.markdown)| |
> ``` lang=cpp, name=Lightning
> function RestoreOrArchetype(name : String, archetype : Archetype, space : Space) : Cog
> ``` 


---  
 #  Store : [StoreResult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#storeresult)

> Store an object.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |object|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function Store(name : String, object : Cog) : StoreResult
> ``` 


---  
 

 
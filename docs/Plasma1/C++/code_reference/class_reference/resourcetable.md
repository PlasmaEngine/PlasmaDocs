 `Resource` `Engine`



(NOTE) A table of resources (or strings) that can be indexed, searched by name, or sampled randomly. The table can be randomly sampled to return an entry into the table.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddOrError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#addorerror-void)|[ All](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#all-plasma-engine-document)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
|[ AddOrIgnore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#addorignore-plasma-engine)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#count-plasma-engine-docume)| | |
|[ AddOrOverwrite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#addoroverwrite-plasma-engi)|[ MaxWeight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#maxweight-plasma-engine-do)| | |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#clear-void)|[ ResourceType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#resourcetype-plasma-engine)| | |
|[ Contains](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#contains-plasma-engine-doc)| | | |
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#createruntime-plasma-engin)| | | |
|[ ForceRebuild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#forcerebuild-void)| | | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#get-plasma-engine-document)| | | |
|[ GetOrDefault](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#getordefault-plasma-engine)| | | |
|[ GetOrError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#getorerror-plasma-engine-d)| | | |
|[ GetOrNull](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#getornull-plasma-engine-do)| | | |
|[ RemoveAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#removeat-void)| | | |
|[ RemoveOrError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#removeorerror-void)| | | |
|[ RemoveOrIgnore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#removeorignore-plasma-engi)| | | |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#runtimeclone-plasma-engine)| | | |
|[ Sample](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#sample-plasma-engine-docum)| | | |
|[ SampleIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#sampleindex-plasma-engine)| | | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md#set-void)| | | |


 #  Properties


---  
 #  All : [resourcetableentryrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentryrange.md)

 `read-only`

> Range to iterate over all entries.
> ``` lang=cpp, name=Lightning
> var All : ResourceTableEntryRange


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> How many items are stored in the table.
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  MaxWeight : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The maximum probability weight value that can be stored in the table. Setting this will clamp all weight values.
> ``` lang=cpp, name=Lightning
> var MaxWeight : Real


---  
 #  ResourceType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> The kind of resource contained in this table. This is either a resource type or "String".
> ``` lang=cpp, name=Lightning
> var ResourceType : String


---  
 #  Methods


---  
 #  AddOrError : Void

> Add the given entry. If another entry with the same name exists then an error is thrown.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function AddOrError(entry : ResourceTableEntry)
> ``` 


---  
 #  AddOrIgnore : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function AddOrIgnore(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  AddOrOverwrite : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then it is overwritten.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function AddOrOverwrite(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  Clear : Void

> Clear all items in the table.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Contains : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns if the given key is contained.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function Contains(key : String) : Boolean
> ``` 


---  
 #  CreateRuntime : [resourcetable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md)

 `static`

> Creates a ResourceTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : ResourceTable
> ``` 


---  
 #  ForceRebuild : Void

> Force rebuild the weighted probability table.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ForceRebuild()
> ``` 


---  
 #  Get : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Hash-Set interface. Gets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function Get(entry : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Hash-Map interface. Gets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function Get(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrDefault : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then the provided default is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |defaultValue|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function GetOrDefault(key : String, defaultValue : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  GetOrError : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetOrError(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrNull : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches then null is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetOrNull(key : String) : ResourceTableEntry
> ``` 


---  
 #  RemoveAt : Void

> Removes the item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveOrError : Void

> Removes the entry associated with the given key. If no entry matches an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveOrError(key : String)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Removes the entry associated with the given key. If no entry matches then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveOrIgnore(key : String) : Boolean
> ``` 


---  
 #  RuntimeClone : [resourcetable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetable.md)

> Creates a clone of this table for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : ResourceTable
> ``` 


---  
 #  Sample : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Samples the table to return a random entry. Takes two (different) random floats from [0,1) in order to sample. Returns an empty string if the table is empty.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |random2|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function Sample(random1 : Real, random2 : Real) : ResourceTableEntry
> ``` 


---  
 #  SampleIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Samples the table to return a random index into the table. Takes two (different) random floats from [0,1) in order to sample.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |random2|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SampleIndex(random1 : Real, random2 : Real) : Integer
> ``` 


---  
 #  Set : Void

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Set interface. Sets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function Set(entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Map interface. Sets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |entry|[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function Set(key : String, entry : ResourceTableEntry)
> ``` 


---  
 

 
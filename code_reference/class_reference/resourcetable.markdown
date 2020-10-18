 `Resource` `Engine`



(NOTE) A table of resources (or strings) that can be indexed, searched by name, or sampled randomly. The table can be randomly sampled to return an entry into the table.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddOrError](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#addorerror-void)|[ All](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#all-plasma-engine-document)|[dataresource](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dataresource.markdown)| |
|[ AddOrIgnore](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#addorignore-plasma-engine)|[ Count](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#count-plasma-engine-docume)| | |
|[ AddOrOverwrite](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#addoroverwrite-plasma-engi)|[ MaxWeight](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#maxweight-plasma-engine-do)| | |
|[ Clear](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#clear-void)|[ ResourceType](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#resourcetype-plasma-engine)| | |
|[ Contains](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#contains-plasma-engine-doc)| | | |
|[ CreateRuntime](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#createruntime-plasma-engin)| | | |
|[ ForceRebuild](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#forcerebuild-void)| | | |
|[ Get](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#get-plasma-engine-document)| | | |
|[ GetOrDefault](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#getordefault-plasma-engine)| | | |
|[ GetOrError](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#getorerror-plasma-engine-d)| | | |
|[ GetOrNull](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#getornull-plasma-engine-do)| | | |
|[ RemoveAt](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#removeat-void)| | | |
|[ RemoveOrError](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#removeorerror-void)| | | |
|[ RemoveOrIgnore](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#removeorignore-plasma-engi)| | | |
|[ RuntimeClone](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#runtimeclone-plasma-engine)| | | |
|[ Sample](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#sample-plasma-engine-docum)| | | |
|[ SampleIndex](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#sampleindex-plasma-engine)| | | |
|[ Set](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown#set-void)| | | |


 #  Properties


---  
 #  All : [resourcetableentryrange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentryrange.markdown)

 `read-only`

> Range to iterate over all entries.
> ``` lang=cpp, name=Lightning
> var All : ResourceTableEntryRange


---  
 #  Count : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> How many items are stored in the table.
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  MaxWeight : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The maximum probability weight value that can be stored in the table. Setting this will clamp all weight values.
> ``` lang=cpp, name=Lightning
> var MaxWeight : Real


---  
 #  ResourceType : [string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

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
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddOrError(entry : ResourceTableEntry)
> ``` 


---  
 #  AddOrIgnore : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Add the given entry. If another entry with the same name exists then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddOrIgnore(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  AddOrOverwrite : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Add the given entry. If another entry with the same name exists then it is overwritten.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
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
 #  Contains : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns if the given key is contained.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Contains(key : String) : Boolean
> ``` 


---  
 #  CreateRuntime : [resourcetable](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown)

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
 #  Get : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Hash-Set interface. Gets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(entry : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Hash-Map interface. Gets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrDefault : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Returns the entry associated with the given key. If no entry matches the key then the provided default is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |defaultValue|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetOrDefault(key : String, defaultValue : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  GetOrError : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Returns the entry associated with the given key. If no entry matches the key then an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetOrError(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrNull : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Returns the entry associated with the given key. If no entry matches then null is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetOrNull(key : String) : ResourceTableEntry
> ``` 


---  
 #  RemoveAt : Void

> Removes the item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveOrError : Void

> Removes the entry associated with the given key. If no entry matches an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveOrError(key : String)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Removes the entry associated with the given key. If no entry matches then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveOrIgnore(key : String) : Boolean
> ``` 


---  
 #  RuntimeClone : [resourcetable](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetable.markdown)

> Creates a clone of this table for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : ResourceTable
> ``` 


---  
 #  Sample : [resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)

> Samples the table to return a random entry. Takes two (different) random floats from [0,1) in order to sample. Returns an empty string if the table is empty.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |random2|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Sample(random1 : Real, random2 : Real) : ResourceTableEntry
> ``` 


---  
 #  SampleIndex : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Samples the table to return a random index into the table. Takes two (different) random floats from [0,1) in order to sample.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |random2|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SampleIndex(random1 : Real, random2 : Real) : Integer
> ``` 


---  
 #  Set : Void

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Set interface. Sets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Map interface. Sets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |entry|[resourcetableentry](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/resourcetableentry.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(key : String, entry : ResourceTableEntry)
> ``` 


---  
 

 
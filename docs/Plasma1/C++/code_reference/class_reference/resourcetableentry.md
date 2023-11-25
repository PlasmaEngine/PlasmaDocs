 `Engine`

(NOTE) An entry from a resource table. The resource type of this entry must match the resource type of the table to add/set. If the value is set via string then the type will be implicitly set to string, otherwise the type must be set via the Resource property.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#clone-plasma-engine-docume)|[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#name-plasma-engine-documen)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#resourcetableentry-void)|[ Resource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#resource-resource)| | |
| |[ ResourceType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#resourcetype-plasma-engine)| | |
| |[ Value](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#value-plasma-engine-docume)| | |
| |[ Weight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md#weight-plasma-engine-docum)| | |


 #  Properties


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Resource : Resource

> The resource value of this entry. Returns null if the underlying type is not a resource. Changes this entry's type to the given resource's type on Set.
> ``` lang=cpp, name=Lightning
> var Resource : Resource


---  
 #  ResourceType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var ResourceType : String


---  
 #  Value : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> The string value of this entry. Changes this entry's type to String on Set.
> ``` lang=cpp, name=Lightning
> var Value : String


---  
 #  Weight : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The weight value used to determine how likely this item is to be sampled. Note: Weights must be positive. Negative weights will be clamped to 0.
> ``` lang=cpp, name=Lightning
> var Weight : Real


---  
 #  Methods


---  
 #  Clone : [resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)

> Creates a new entry with the same values.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : ResourceTableEntry
> ``` 


---  
 #  ResourceTableEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ResourceTableEntry()
> ``` 


---  
 #  ResourceTableEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[resourcetableentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Lightning
> function ResourceTableEntry( : ResourceTableEntry)
> ``` 


---  
 

 
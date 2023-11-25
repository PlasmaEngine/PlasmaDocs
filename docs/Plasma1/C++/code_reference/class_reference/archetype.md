 `Resource` `Engine`



(NOTE) An archetype is a resource containing the serialized data definition of an object. The archetype stores a binary cache of the serialization data and the source file for debugging and for archetype updating.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ StoredType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md#storedtype-plasma-engine-d)|Resource| |


 #  Properties


---  
 #  StoredType : [boundtype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boundtype.md)

> An Archetype can be a Cog, Space, or GameSession. It's okay for this to be a raw BoundType* because native types will never be destructed.
> ``` lang=cpp, name=Lightning
> var StoredType : BoundType


---  
 #  Methods


---  
 

 
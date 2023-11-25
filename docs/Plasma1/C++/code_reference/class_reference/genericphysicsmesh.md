 `Resource` `Physics`



(NOTE) Base class of mesh type physics resources. Stores the actual mesh (no optimization structures) and information about the mesh such as mass and inertia.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ UpdateAndNotifyIfModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/genericphysicsmesh.md#updateandnotifyifmodifie)|[ Indices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/genericphysicsmesh.md#indices-plasma-engine-docu)|Resource|[convexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.md)|
|[ Validate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/genericphysicsmesh.md#validate-plasma-engine-doc)|[ Vertices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/genericphysicsmesh.md#vertices-plasma-engine-doc)| |[physicsmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmesh.md)|


 #  Properties


---  
 #  Indices : [physicsmeshindexdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmeshindexdata.md)

 `read-only`

> The index buffer data of this mesh.
> ``` lang=cpp, name=Lightning
> var Indices : PhysicsMeshIndexData


---  
 #  Vertices : [physicsmeshvertexdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmeshvertexdata.md)

 `read-only`

> The vertex buffer data of this mesh.
> ``` lang=cpp, name=Lightning
> var Vertices : PhysicsMeshVertexData


---  
 #  Methods


---  
 #  UpdateAndNotifyIfModified : Void

> Rebuild all extra mesh information if it is currently modified. This includes things like the center of mass, volume, aabb, edge info and more (some derived types may have a mid-phase, etc...)
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UpdateAndNotifyIfModified()
> ``` 


---  
 #  Validate : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Check if the mesh is valid. Optionally throw a script exception if it is invalid.
> |Name|Type|Description|
> |---|---|---|
> |throwExceptionIfInvalid|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function Validate(throwExceptionIfInvalid : Boolean) : Boolean
> ``` 


---  
 

 
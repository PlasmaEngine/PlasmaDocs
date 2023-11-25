 `Resource` `Physics`



(NOTE) Represents a collection of convex meshes that was decomposed from a mesh.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#createruntime-plasma-engin)|[ Modified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#modified-plasma-engine-doc)|Resource| |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#runtimeclone-plasma-engine)|[ SubMeshes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#submeshes-plasma-engine-do)| | |
|[ UpdateAndNotifyIfModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#updateandnotifyifmodifie)|[ Valid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#valid-plasma-engine-docume)| | |
|[ Validate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#validate-plasma-engine-doc)|[ Vertices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md#vertices-plasma-engine-doc)| | |


 #  Properties


---  
 #  Modified : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Is the resource currently modified?
> ``` lang=cpp, name=Lightning
> var Modified : Boolean


---  
 #  SubMeshes : [multiconvexmeshsubmeshdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.md)

 `read-only`

> A collection of sub-convex meshes.
> ``` lang=cpp, name=Lightning
> var SubMeshes : MultiConvexMeshSubMeshData


---  
 #  Valid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Is the resource correctly setup? Typically involves a mis-match in indices and vertices.
> ``` lang=cpp, name=Lightning
> var Valid : Boolean


---  
 #  Vertices : [multiconvexmeshvertexdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshvertexdata.md)

 `read-only`

> The vertex buffer data of this mesh.
> ``` lang=cpp, name=Lightning
> var Vertices : MultiConvexMeshVertexData


---  
 #  Methods


---  
 #  CreateRuntime : [multiconvexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md)

 `static`

> Creates a MultiConvexMesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : MultiConvexMesh
> ``` 


---  
 #  RuntimeClone : [multiconvexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md)

> Creates a clone of this mesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : MultiConvexMesh
> ``` 


---  
 #  UpdateAndNotifyIfModified : Void

> Rebuild all extra mesh information if it is currently modified. This includes things like the center of mass, volume, aabb, edge info and more.
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
 

 
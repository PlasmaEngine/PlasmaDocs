 `Component` `Physics`



(NOTE) Defines the collision for a generic mesh from a collection of triangles ( PhysicsMesh resource). This collider type is not expected to have a dynamic or kinematic RigidBody.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md#meshcollider-void)|[ DrawEdges](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md#drawedges-plasma-engine-do)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
| |[ DrawFaceNormals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md#drawfacenormals-plasma-eng)| | |
| |[ DrawFaces](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md#drawfaces-plasma-engine-do)| | |
| |[ PhysicsMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md#physicsmesh-plasma-engine)| | |


 #  Properties


---  
 #  DrawEdges : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether to debug draw the edges of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawEdges : Boolean


---  
 #  DrawFaceNormals : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether to debug draw the normals of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawFaceNormals : Boolean


---  
 #  DrawFaces : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether to debug draw the faces of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawFaces : Boolean


---  
 #  PhysicsMesh : [physicsmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmesh.md)

> The mesh resource used to define collision. This mesh is just a surface mesh of triangles (no volume is defined).
> ``` lang=cpp, name=Lightning
> var PhysicsMesh : PhysicsMesh


---  
 #  Methods


---  
 #  MeshCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MeshCollider()
> ``` 


---  
 

 
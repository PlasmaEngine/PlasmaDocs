 `Component` `Physics`



(NOTE) Defines the collision for a generic mesh from a collection of triangles ( PhysicsMesh resource). This collider type is not expected to have a dynamic or kinematic RigidBody.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown#meshcollider-void)|[ DrawEdges](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown#drawedges-plasma-engine-do)|[collider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown)| |
| |[ DrawFaceNormals](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown#drawfacenormals-plasma-eng)| | |
| |[ DrawFaces](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown#drawfaces-plasma-engine-do)| | |
| |[ PhysicsMesh](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown#physicsmesh-plasma-engine)| | |


 #  Properties


---  
 #  DrawEdges : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether to debug draw the edges of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawEdges : Boolean


---  
 #  DrawFaceNormals : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether to debug draw the normals of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawFaceNormals : Boolean


---  
 #  DrawFaces : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether to debug draw the faces of each triangle.
> ``` lang=cpp, name=Lightning
> var DrawFaces : Boolean


---  
 #  PhysicsMesh : [physicsmesh](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicsmesh.markdown)

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
 

 
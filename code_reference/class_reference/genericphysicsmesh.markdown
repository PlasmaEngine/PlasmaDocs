 `Resource` `Physics`



(NOTE) Base class of mesh type physics resources. Stores the actual mesh (no optimization structures) and information about the mesh such as mass and inertia.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ UpdateAndNotifyIfModified](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/genericphysicsmesh.markdown#updateandnotifyifmodifie)|[ Indices](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/genericphysicsmesh.markdown#indices-plasma-engine-docu)|Resource|[convexmesh](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/convexmesh.markdown)|
|[ Validate](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/genericphysicsmesh.markdown#validate-plasma-engine-doc)|[ Vertices](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/genericphysicsmesh.markdown#vertices-plasma-engine-doc)| |[physicsmesh](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicsmesh.markdown)|


 #  Properties


---  
 #  Indices : [physicsmeshindexdata](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicsmeshindexdata.markdown)

 `read-only`

> The index buffer data of this mesh.
> ``` lang=cpp, name=Lightning
> var Indices : PhysicsMeshIndexData


---  
 #  Vertices : [physicsmeshvertexdata](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicsmeshvertexdata.markdown)

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
 #  Validate : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Check if the mesh is valid. Optionally throw a script exception if it is invalid.
> |Name|Type|Description|
> |---|---|---|
> |throwExceptionIfInvalid|[boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Validate(throwExceptionIfInvalid : Boolean) : Boolean
> ``` 


---  
 

 
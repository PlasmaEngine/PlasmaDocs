 `Physics`



(NOTE) Contains the indices of a convex mesh. The triangle indices are the primary method to configure this (required for mass computations). The regular indices are used for debug drawing and to reduce intersection tests by removing duplicate points. If left empty, Indices will be auto-filled from the triangle indices.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Indices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.md#indices-plasma-engine-docu)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.md)| |
| |[ Mesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.md#mesh-plasma-engine-documen)| | |
| |[ TriangleIndices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.md#triangleindices-plasma-eng)| | |
| |[ Valid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.md#valid-plasma-engine-docume)| | |


 #  Properties


---  
 #  Indices : [multiconvexmeshindexdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshindexdata.md)

 `read-only`

> The vertex indices on the main mesh used to generate the convex hull.
> ``` lang=cpp, name=Lightning
> var Indices : MultiConvexMeshIndexData


---  
 #  Mesh : [multiconvexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md)

> The MultiConvexMesh that owns this sub-mesh.
> ``` lang=cpp, name=Lightning
> var Mesh : MultiConvexMesh


---  
 #  TriangleIndices : [multiconvexmeshindexdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshindexdata.md)

 `read-only`

> The vertex indices on the main mesh used to generate triangle indices for computing mass information and debug drawing. More indices are needed for determining triangles than for generating the convex mesh.
> ``` lang=cpp, name=Lightning
> var TriangleIndices : MultiConvexMeshIndexData


---  
 #  Valid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Is this sub-mesh incorrectly configured. Typically means that the indices don't point to valid vertices. Also the number of triangle indices could be incorrect (multiple of 3).
> ``` lang=cpp, name=Lightning
> var Valid : Boolean


---  
 #  Methods


---  
 

 
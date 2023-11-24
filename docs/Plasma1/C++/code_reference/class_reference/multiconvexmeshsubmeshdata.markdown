 `Physics`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#add-plasma-engine-document)|[ All](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#all-plasma-engine-document)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.markdown)| |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#clear-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#count-plasma-engine-docume)| | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#get-plasma-engine-document)| | | |
|[ RemoveAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshdata.markdown#removeat-void)| | | |


 #  Properties


---  
 #  All : [multiconvexmeshsubmeshrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshsubmeshrange.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var All : MultiConvexMeshSubMeshRange


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  Methods


---  
 #  Add : [subconvexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.markdown)

> Create and add a new SubConvexMesh. Returns the new mesh for modification.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Add() : SubConvexMesh
> ``` 


---  
 #  Clear : Void

> Clears all sub-meshes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Get : [subconvexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subconvexmesh.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get( : Integer) : SubConvexMesh
> ``` 


---  
 #  RemoveAt : Void

> Remove the sub-mesh at the given index.
> |Name|Type|Description|
> |---|---|---|
> |arrayIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveAt(arrayIndex : Integer)
> ``` 


---  
 

 
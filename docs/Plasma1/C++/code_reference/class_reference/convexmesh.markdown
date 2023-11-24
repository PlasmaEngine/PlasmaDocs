 `Resource` `Physics`



(NOTE) A convex mesh meant for use with dynamic rigid bodies. Computes efficient contact information compared to a regular physics mesh. This mesh also defines a volume which means mass properties can be computed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.markdown#convexmesh-void)| |[genericphysicsmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/genericphysicsmesh.markdown)| |
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.markdown#createruntime-plasma-engin)| | | |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.markdown#runtimeclone-plasma-engine)| | | |


 #  Properties


---  
 #  Methods


---  
 #  ConvexMesh : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ConvexMesh()
> ``` 


---  
 #  CreateRuntime : [convexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.markdown)

 `static`

> Creates a ConvexMesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : ConvexMesh
> ``` 


---  
 #  RuntimeClone : [convexmesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.markdown)

> Creates a clone of this mesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : ConvexMesh
> ``` 


---  
 

 
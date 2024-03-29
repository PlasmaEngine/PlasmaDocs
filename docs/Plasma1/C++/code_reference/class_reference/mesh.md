 `Resource` `Graphics`



(NOTE) Data that represents a mesh in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#createruntime-plasma-engin)|[ Indices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#indices-plasma-engine-docu)|Resource| |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#runtimeclone-plasma-engine)|[ PrimitiveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#primitivetype-plasma-engin)| | |
|[ Upload](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#upload-void)|[ Vertices](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#vertices-plasma-engine-doc)| | |
|[ UploadNoRayCastInfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#uploadnoraycastinfo-void)| | | |
|[ UploadNoRayCastInfoOrAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md#uploadnoraycastinfooraab)| | | |


 #  Properties


---  
 #  Indices : [indexbuffer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/indexbuffer.md)

 `read-only`

> Indices used to define non-sequential primitive construction from vertices, such as shared vertices.
> ``` lang=cpp, name=Lightning
> var Indices : IndexBuffer


---  
 #  PrimitiveType : [PrimitiveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#primitivetype)

> The type of primitives to be made with the vertex data.
> ``` lang=cpp, name=Lightning
> var PrimitiveType : PrimitiveType


---  
 #  Vertices : [vertexbuffer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md)

 `read-only`

> Vertex data and attribute semantics for defining data that can be uploaded to the gpu.
> ``` lang=cpp, name=Lightning
> var Vertices : VertexBuffer


---  
 #  Methods


---  
 #  CreateRuntime : [mesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md)

 `static`

> Makes an anonymous Mesh resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : Mesh
> ``` 


---  
 #  RuntimeClone : [mesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md)

> Creates a clone of this Mesh. As a clone is expected to be modified, an upload function must be called before this mesh can be used.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : Mesh
> ``` 


---  
 #  Upload : Void

> Upload vertex buffer and index buffer data to the gpu. This will also build the aabb and information needed for raycasting.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Upload()
> ``` 


---  
 #  UploadNoRayCastInfo : Void

> Same as Upload except raycasting information will not be built. This avoids a possible spike when a custom mesh will never need to be raycasted against.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UploadNoRayCastInfo()
> ``` 


---  
 #  UploadNoRayCastInfoOrAabb : Void

> Same as Upload except raycasting information and the aabb will not be built. This should be used when the user is manually setting an aabb or frustum culling is disabled.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UploadNoRayCastInfoOrAabb()
> ``` 


---  
 

 
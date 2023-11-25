 `Graphics`

(NOTE) Vertex data and attribute semantics for defining data that can be uploaded to the gpu.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddAttribute](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#addattribute-void)|[ VertexCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#vertexcount-plasma-engine)|[safeid32](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32.md)| |
|[ AddByte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#addbyte-void)| | | |
|[ AddReal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#addreal-void)| | | |
|[ AddShort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#addshort-void)| | | |
|[ ClearAttributes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#clearattributes-void)| | | |
|[ ClearData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#cleardata-void)| | | |
|[ GetAttributes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#getattributes-plasma-engin)| | | |
|[ GetElementCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#getelementcount-plasma-eng)| | | |
|[ GetElementType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#getelementtype-plasma-engi)| | | |
|[ GetVertexData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#getvertexdata-plasma-engin)| | | |
|[ IsValidVertexData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexbuffer.md#isvalidvertexdata-plasma-e)| | | |


 #  Properties


---  
 #  VertexCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the number of vertices that have a complete set of data stored.
> ``` lang=cpp, name=Lightning
> var VertexCount : Integer


---  
 #  Methods


---  
 #  AddAttribute : Void

> Adds an attribute to the definition of the vertices that are to be stored. Add the attributes in the order that they should be stored in memory on a vertex.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> |elementType|[VertexElementType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexelementtype)| |
> |elementCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function AddAttribute(semantic : VertexSemantic, elementType : VertexElementType, elementCount : Integer)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function AddByte(value : Integer)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)| |
> ``` lang=cpp, name=Lightning
> function AddByte( : Integer2)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer3.md)| |
> ``` lang=cpp, name=Lightning
> function AddByte( : Integer3)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer4.md)| |
> ``` lang=cpp, name=Lightning
> function AddByte( : Integer4)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function AddReal(value : Real)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)| |
> ``` lang=cpp, name=Lightning
> function AddReal(value : Real2)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function AddReal(value : Real3)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function AddReal(value : Real4)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function AddShort(value : Integer)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)| |
> ``` lang=cpp, name=Lightning
> function AddShort( : Integer2)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer3.md)| |
> ``` lang=cpp, name=Lightning
> function AddShort( : Integer3)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer4.md)| |
> ``` lang=cpp, name=Lightning
> function AddShort( : Integer4)
> ``` 


---  
 #  ClearAttributes : Void

> Clears all added attributes from the vertex definition so they can be redefined.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearAttributes()
> ``` 


---  
 #  ClearData : Void

> Clears all added vertex data so new data can be added.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearData()
> ``` 


---  
 #  GetAttributes : [vertexsemanticrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vertexsemanticrange.md)

> Returns a range of attribute semantics in the order that they were added.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetAttributes() : VertexSemanticRange
> ``` 


---  
 #  GetElementCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Returns the number of elements stored for the given attribute, throws exception if the attribute is not in the vertex definition.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Lightning
> function GetElementCount(semantic : VertexSemantic) : Integer
> ``` 


---  
 #  GetElementType : [VertexElementType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexelementtype)

> Returns the type that is used to store the given attribute, throws exception if the attribute is not in the vertex definition.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Lightning
> function GetElementType(semantic : VertexSemantic) : VertexElementType
> ``` 


---  
 #  GetVertexData : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Gets the data of an attribute of a vertex, returns values of 0 if read is invalid.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Lightning
> function GetVertexData(vertexIndex : Integer, semantic : VertexSemantic) : Real4
> ``` 


---  
 #  GetVertexData : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Gets the data of an attribute of a vertex, throws exception if attribute info doesn't match or read is invalid.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> |type|[VertexElementType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexelementtype)| |
> |count|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetVertexData(vertexIndex : Integer, semantic : VertexSemantic, type : VertexElementType, count : Integer) : Real4
> ``` 


---  
 #  IsValidVertexData : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns false if GetVertexData() would throw an exception with the same arguments.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |semantic|[VertexSemantic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexsemantic)| |
> |type|[VertexElementType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#vertexelementtype)| |
> |count|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IsValidVertexData(vertexIndex : Integer, semantic : VertexSemantic, type : VertexElementType, count : Integer) : Boolean
> ``` 


---  
 

 
 `Graphics`

(NOTE) Indices used to define non-sequential primitive construction from vertices, such as shared vertices.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/indexbuffer.markdown#add-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/indexbuffer.markdown#count-plasma-engine-docume)|[safeid32](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32.markdown)| |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/indexbuffer.markdown#clear-void)| | | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/indexbuffer.markdown#get-plasma-engine-document)| | | |


 #  Properties


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Number of vertex indices currently in buffer. Can be set manually to invoke vertex shading that number of times, with or without vertex data.
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  Methods


---  
 #  Add : Void

> Add a vertex index to the buffer.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Add(value : Integer)
> ``` 


---  
 #  Clear : Void

> Clears all stored indices so that new ones can be added.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Get : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Returns the vertex index that is stored at the given index of this buffer.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : Integer
> ``` 


---  
 

 
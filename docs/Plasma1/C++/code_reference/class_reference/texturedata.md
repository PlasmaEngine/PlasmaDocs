 `Graphics`

(NOTE) Modifiable texture data that can be used to upload to a runtime Texture resource. All formats use one interface for get/set, all values are converted to/from floats and unused channels are ignored. Integer formats are represented in the normalized range [0, 1].

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#get-plasma-engine-document)|[ Format](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#format-plasma-engine-docum)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#set-void)|[ Height](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#height-plasma-engine-docum)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#texturedata-void)|[ PixelCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#pixelcount-plasma-engine-d)| | |
| |[ Width](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md#width-plasma-engine-docume)| | |


 #  Properties


---  
 #  Format : [TextureFormat](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data.
> ``` lang=cpp, name=Lightning
> var Format : TextureFormat


---  
 #  Height : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Height of the texture data in pixels.
> ``` lang=cpp, name=Lightning
> var Height : Integer


---  
 #  PixelCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Total number of pixels in texture data.
> ``` lang=cpp, name=Lightning
> var PixelCount : Integer


---  
 #  Width : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Width of the texture data in pixels.
> ``` lang=cpp, name=Lightning
> var Width : Integer


---  
 #  Methods


---  
 #  Get : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : Real4
> ``` 


---  
 #  Get : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |y|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(x : Integer, y : Integer) : Real4
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |y|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |value|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function Set(x : Integer, y : Integer, value : Real4)
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |value|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, value : Real4)
> ``` 


---  
 #  TextureData : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[TextureFormat](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureformat)| |
> |width|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |height|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function TextureData(format : TextureFormat, width : Integer, height : Integer)
> ``` 


---  
 

 
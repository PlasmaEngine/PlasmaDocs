 `Graphics`

(NOTE) Modifiable texture data that can be used to upload to a runtime Texture resource. All formats use one interface for get/set, all values are converted to/from floats and unused channels are ignored. Integer formats are represented in the normalized range [0, 1].

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#get-plasma-engine-document)|[ Format](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#format-plasma-engine-docum)| | |
|[ Set](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#set-void)|[ Height](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#height-plasma-engine-docum)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#texturedata-void)|[ PixelCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#pixelcount-plasma-engine-d)| | |
| |[ Width](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/texturedata.markdown#width-plasma-engine-docume)| | |


 #  Properties


---  
 #  Format : [TextureFormat](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#textureformat)

 `read-only`

> Memory format of the stored pixel data.
> ``` lang=cpp, name=Lightning
> var Format : TextureFormat


---  
 #  Height : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Height of the texture data in pixels.
> ``` lang=cpp, name=Lightning
> var Height : Integer


---  
 #  PixelCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Total number of pixels in texture data.
> ``` lang=cpp, name=Lightning
> var PixelCount : Integer


---  
 #  Width : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Width of the texture data in pixels.
> ``` lang=cpp, name=Lightning
> var Width : Integer


---  
 #  Methods


---  
 #  Get : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : Real4
> ``` 


---  
 #  Get : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(x : Integer, y : Integer) : Real4
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |value|[real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(x : Integer, y : Integer, value : Real4)
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |value|[real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, value : Real4)
> ``` 


---  
 #  TextureData : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[TextureFormat](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#textureformat)| |
> |width|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |height|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function TextureData(format : TextureFormat, width : Integer, height : Integer)
> ``` 


---  
 

 
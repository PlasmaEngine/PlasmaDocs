 `Resource` `Graphics`



(NOTE) Data that represents a texture in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#createruntime-plasma-engin)|[ AddressingX](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#addressingx-plasma-engine)|Resource| |
|[ SubUpload](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#subupload-void)|[ AddressingY](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#addressingy-plasma-engine)| | |
|[ Upload](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#upload-void)|[ Anisotropy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#anisotropy-plasma-engine-d)| | |
| |[ CompareFunc](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#comparefunc-plasma-engine)| | |
| |[ CompareMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#comparemode-plasma-engine)| | |
| |[ Compression](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#compression-plasma-engine)| | |
| |[ Filtering](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#filtering-plasma-engine-do)| | |
| |[ Format](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#format-plasma-engine-docum)| | |
| |[ Height](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#height-plasma-engine-docum)| | |
| |[ MipMapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#mipmapping-plasma-engine-d)| | |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#size-plasma-engine-documen)| | |
| |[ Type](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#type-plasma-engine-documen)| | |
| |[ Width](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md#width-plasma-engine-docume)| | |


 #  Properties


---  
 #  AddressingX : [TextureAddressing](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's width.
> ``` lang=cpp, name=Lightning
> var AddressingX : TextureAddressing


---  
 #  AddressingY : [TextureAddressing](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's height.
> ``` lang=cpp, name=Lightning
> var AddressingY : TextureAddressing


---  
 #  Anisotropy : [TextureAnisotropy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureanisotropy)

> Max ratio of anisotropy that filtering will account for at oblique viewing angles.
> ``` lang=cpp, name=Lightning
> var Anisotropy : TextureAnisotropy


---  
 #  CompareFunc : [TextureCompareFunc](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturecomparefunc)

> Which method of comparison should be used if CompareMode is set to Enable.
> ``` lang=cpp, name=Lightning
> var CompareFunc : TextureCompareFunc


---  
 #  CompareMode : [TextureCompareMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturecomparemode)

> If sampling in hardware should perform comparison instead of fetching. Requires using SamplerShadow2d in the shader.
> ``` lang=cpp, name=Lightning
> var CompareMode : TextureCompareMode


---  
 #  Compression : [TextureCompression](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturecompression)

 `read-only`

> Block compression method being used. Requires pre-processing, cannot be set for runtime Textures.
> ``` lang=cpp, name=Lightning
> var Compression : TextureCompression


---  
 #  Filtering : [TextureFiltering](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturefiltering)

> How samples should be blended under minification/magnification.
> ``` lang=cpp, name=Lightning
> var Filtering : TextureFiltering


---  
 #  Format : [TextureFormat](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Lightning
> var Format : TextureFormat


---  
 #  Height : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Height of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Lightning
> var Height : Integer


---  
 #  MipMapping : [TextureMipMapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturemipmapping)

> If downsampled versions of the texture (mip maps) should be generated. PreGenerated is not valid for runtime Textures.
> ``` lang=cpp, name=Lightning
> var MipMapping : TextureMipMapping


---  
 #  Size : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

 `read-only`

> Width and height (x, y) of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Lightning
> var Size : Integer2


---  
 #  Type : [TextureType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturetype)

 `read-only`

> The type of texture data being represented.
> ``` lang=cpp, name=Lightning
> var Type : TextureType


---  
 #  Width : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Width of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Lightning
> var Width : Integer


---  
 #  Methods


---  
 #  CreateRuntime : [texture](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texture.md)

 `static`

> Makes an anonymous Texture resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : Texture
> ``` 


---  
 #  SubUpload : Void

> Uploads the given texture data, overwriting a sub region of the texture data that is already on the gpu.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md)| |
> |xOffset|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |yOffset|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function SubUpload(textureData : TextureData, xOffset : Integer, yOffset : Integer)
> ``` 


---  
 #  Upload : Void

> Uploads the given texture data to the gpu, configured with the current settings of this Texture.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texturedata.md)| |
> ``` lang=cpp, name=Lightning
> function Upload(textureData : TextureData)
> ``` 


---  
 

 
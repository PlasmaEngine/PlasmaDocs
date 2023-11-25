 `Graphics`

(NOTE) Used when requesting a RenderTarget to configure how its texture is sampled.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#samplersettings-void)|[ AddressingX](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#addressingx-plasma-engine)| | |
| |[ AddressingY](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#addressingy-plasma-engine)| | |
| |[ CompareFunc](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#comparefunc-plasma-engine)| | |
| |[ CompareMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#comparemode-plasma-engine)| | |
| |[ Filtering](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplersettings.md#filtering-plasma-engine-do)| | |


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
 #  Filtering : [TextureFiltering](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturefiltering)

> How samples should be blended under minification/magnification.
> ``` lang=cpp, name=Lightning
> var Filtering : TextureFiltering


---  
 #  Methods


---  
 #  SamplerSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SamplerSettings()
> ``` 


---  
 

 
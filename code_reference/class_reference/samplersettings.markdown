 `Graphics`

(NOTE) Used when requesting a RenderTarget to configure how its texture is sampled.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#samplersettings-void)|[ AddressingX](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#addressingx-plasma-engine)| | |
| |[ AddressingY](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#addressingy-plasma-engine)| | |
| |[ CompareFunc](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#comparefunc-plasma-engine)| | |
| |[ CompareMode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#comparemode-plasma-engine)| | |
| |[ Filtering](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/samplersettings.markdown#filtering-plasma-engine-do)| | |


 #  Properties


---  
 #  AddressingX : [TextureAddressing](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's width.
> ``` lang=cpp, name=Lightning
> var AddressingX : TextureAddressing


---  
 #  AddressingY : [TextureAddressing](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's height.
> ``` lang=cpp, name=Lightning
> var AddressingY : TextureAddressing


---  
 #  CompareFunc : [TextureCompareFunc](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#texturecomparefunc)

> Which method of comparison should be used if CompareMode is set to Enable.
> ``` lang=cpp, name=Lightning
> var CompareFunc : TextureCompareFunc


---  
 #  CompareMode : [TextureCompareMode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#texturecomparemode)

> If sampling in hardware should perform comparison instead of fetching. Requires using SamplerShadow2d in the shader.
> ``` lang=cpp, name=Lightning
> var CompareMode : TextureCompareMode


---  
 #  Filtering : [TextureFiltering](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#texturefiltering)

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
 

 
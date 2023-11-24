 `Graphics`

(NOTE) Contains all output targets and render settings needed for a render task.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#rendersettings-void)|[ BlendSettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#blendsettings-plasma-engin)| | |
| |[ ColorTarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#colortarget-plasma-engine)| | |
| |[ CullMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#cullmode-plasma-engine-doc)| | |
| |[ DepthSettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#depthsettings-plasma-engin)| | |
| |[ DepthTarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#depthtarget-plasma-engine)| | |
| |[ GlobalShaderInputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#globalshaderinputs-plasma)| | |
| |[ MultiRenderTarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown#multirendertarget-plasma-e)| | |


 #  Properties


---  
 #  BlendSettings : [blendsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/blendsettings.markdown)

> Settings to use when blending shader output with the ColorTarget, implicitly BlendSettings0.
> ``` lang=cpp, name=Lightning
> var BlendSettings : BlendSettings


---  
 #  ColorTarget : [rendertarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendertarget.markdown)

> The RenderTarget of a color format to output to, implicitly RenderTarget0.
> ``` lang=cpp, name=Lightning
> var ColorTarget : RenderTarget


---  
 #  CullMode : [CullMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#cullmode)

> 
> ``` lang=cpp, name=Lightning
> var CullMode : CullMode


---  
 #  DepthSettings : [depthsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/depthsettings.markdown)

> Settings to use when doing depth/stencil testing with DepthTarget.
> ``` lang=cpp, name=Lightning
> var DepthSettings : DepthSettings


---  
 #  DepthTarget : [rendertarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendertarget.markdown)

> The RenderTarget of a depth format to use as a depth buffer for depth/stencil testing.
> ``` lang=cpp, name=Lightning
> var DepthTarget : RenderTarget


---  
 #  GlobalShaderInputs : [shaderinputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/shaderinputs.markdown)

> Shader input values to be globally overridden for all objects/shaders.
> ``` lang=cpp, name=Lightning
> var GlobalShaderInputs : ShaderInputs


---  
 #  MultiRenderTarget : [multirendertarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multirendertarget.markdown)

 `read-only`

> Interface for configuring multiple color target outputs.
> ``` lang=cpp, name=Lightning
> var MultiRenderTarget : MultiRenderTarget


---  
 #  Methods


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RenderSettings()
> ``` 


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[rendersettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.markdown)| |
> ``` lang=cpp, name=Lightning
> function RenderSettings( : RenderSettings)
> ``` 


---  
 

 
 `Component` `Graphics`



(NOTE) Base interface for components that require rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ GroupSortValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#groupsortvalue-plasma-engi)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)|[basesprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basesprite.md)|
| |[ LocalAabbCenter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#localaabbcenter-plasma-eng)| |[debuggraphical](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debuggraphical.md)|
| |[ LocalAabbHalfExtents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#localaabbhalfextents-zer)| |[heightmapmodel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapmodel.md)|
| |[ Material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#material-plasma-engine-doc)| |[model](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/model.md)|
| |[ OverrideBoundingBox](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#overrideboundingbox-plasma)| |[particlesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md)|
| |[ ShaderInputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#shaderinputs-plasma-engine)| |[skinnedmodel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/skinnedmodel.md)|
| |[ ViewCulling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#viewculling-plasma-engine)| | |
| |[ VisibilityEvents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#visibilityevents-plasma-en)| | |
| |[ Visible](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#visible-plasma-engine-docu)| | |
| |[ WorldAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md#worldaabb-plasma-engine-do)| | |


 #  Properties


---  
 #  GroupSortValue : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Can be used by a RenderGroup to define draw order, from lowest to highest.
> ``` lang=cpp, name=Lightning
> var GroupSortValue : Integer


---  
 #  LocalAabbCenter : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Center of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Lightning
> var LocalAabbCenter : Real3


---  
 #  LocalAabbHalfExtents : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Half extents of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Lightning
> var LocalAabbHalfExtents : Real3


---  
 #  Material : [material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md)

> The composition of shader fragments that determines how the graphical is rendered.
> ``` lang=cpp, name=Lightning
> var Material : Material


---  
 #  OverrideBoundingBox : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Manually set the bounding box that is used for frustum culling.
> ``` lang=cpp, name=Lightning
> var OverrideBoundingBox : Boolean


---  
 #  ShaderInputs : [shaderinputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/shaderinputs.md)

> List of shader inputs to be manually overridden only on this object.
> ``` lang=cpp, name=Lightning
> var ShaderInputs : ShaderInputs


---  
 #  ViewCulling : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If the graphical should not be drawn when its bounding volume is outside of the view frustum.
> ``` lang=cpp, name=Lightning
> var ViewCulling : Boolean


---  
 #  VisibilityEvents : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If object receives events when entering/exiting the view of an active camera.
> ``` lang=cpp, name=Lightning
> var VisibilityEvents : Boolean


---  
 #  Visible : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If the graphical should be drawn.
> ``` lang=cpp, name=Lightning
> var Visible : Boolean


---  
 #  WorldAabb : [aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)

 `read-only`

> The world space axis aligned bounding volume that is used for frustum culling.
> ``` lang=cpp, name=Lightning
> var WorldAabb : Aabb


---  
 #  Methods


---  
 

 
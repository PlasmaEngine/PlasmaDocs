 `Component` `Physics`



(NOTE) Common interface for all point effects. Used to attract or repel objects towards a central point. The strength of the effect is calculated as an interpolation between two strength values at two radial distances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ EndCondition](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#endcondition-plasma-engine)|[physicseffect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicseffect.markdown)|[pointforceeffect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/pointforceeffect.markdown)|
| |[ InterpolationType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#interpolationtype-plasma-e)| |[pointgravityeffect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/pointgravityeffect.markdown)|
| |[ LocalPositionOffset](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#localpositionoffset-plasma)| | |
| |[ MaxDistance](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#maxdistance-plasma-engine)| | |
| |[ MinDistance](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#mindistance-plasma-engine)| | |
| |[ StrengthAtMax](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#strengthatmax-plasma-engin)| | |
| |[ StrengthAtMin](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basicpointeffect.markdown#strengthatmin-plasma-engin)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#physicseffectendcondition)

> How the interpolation should be handled after max distance. ClampToMax will clamp to StrengthAtMax. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ``` lang=cpp, name=Lightning
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the effect.
> ``` lang=cpp, name=Lightning
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  LocalPositionOffset : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The offset from the transform position (in local space) that the point effect will be applied at.
> ``` lang=cpp, name=Lightning
> var LocalPositionOffset : Real3


---  
 #  MaxDistance : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ``` lang=cpp, name=Lightning
> var MaxDistance : Real


---  
 #  MinDistance : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The first distance at which attenuation will start. If an object is under the min distance, StrengthAtMin will be used. If an object is in between min and max, then it will attenuate.
> ``` lang=cpp, name=Lightning
> var MinDistance : Real


---  
 #  StrengthAtMax : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The strength that this effect applies at the max distance.
> ``` lang=cpp, name=Lightning
> var StrengthAtMax : Real


---  
 #  StrengthAtMin : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The strength that this effect applies at the min distance.
> ``` lang=cpp, name=Lightning
> var StrengthAtMin : Real


---  
 #  Methods


---  
 

 
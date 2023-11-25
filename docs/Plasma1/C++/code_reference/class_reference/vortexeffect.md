 `Component` `Physics`



(NOTE) Applies a force about an axis at the object's center. This will apply two forces to a body: One pulls the object towards the center of the vortex and the other applies a tangential force. Useful to model a vortex. This only expects to be used as a Region effect.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#vortexeffect-void)|[ EndCondition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#endcondition-plasma-engine)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)| |
| |[ InterpolationType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#interpolationtype-plasma-e)| | |
| |[ InwardStrengthAtMaxDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#inwardstrengthatmaxdista)| | |
| |[ InwardStrengthAtMinDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#inwardstrengthatmindista)| | |
| |[ LocalAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#localaxis-plasma-engine-do)| | |
| |[ MaxDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#maxdistance-plasma-engine)| | |
| |[ MinDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#mindistance-plasma-engine)| | |
| |[ TwistStrengthAtMaxDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#twiststrengthatmaxdistan)| | |
| |[ TwistStrengthAtMinDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#twiststrengthatmindistan)| | |
| |[ VortexAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#vortexaxis-plasma-engine-d)| | |
| |[ WorldVortexAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.md#worldvortexaxis-plasma-eng)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#physicseffectendcondition)

> How the interpolation should be handled at MaxDistance. ClampToMax will clamp to the max strength values. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ``` lang=cpp, name=Lightning
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the forces.
> ``` lang=cpp, name=Lightning
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  InwardStrengthAtMaxDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The inward strength of the vortex at the max distance.
> ``` lang=cpp, name=Lightning
> var InwardStrengthAtMaxDistance : Real


---  
 #  InwardStrengthAtMinDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The inward strength of the vortex at the min distance.
> ``` lang=cpp, name=Lightning
> var InwardStrengthAtMinDistance : Real


---  
 #  LocalAxis : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the vortex axis is in world or local space.
> ``` lang=cpp, name=Lightning
> var LocalAxis : Boolean


---  
 #  MaxDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ``` lang=cpp, name=Lightning
> var MaxDistance : Real


---  
 #  MinDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The first distance at which attenuation will start. If an object is under the min distance, the min strength values will be used. If an object is in between min and max, then it will attenuate.
> ``` lang=cpp, name=Lightning
> var MinDistance : Real


---  
 #  TwistStrengthAtMaxDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The perpendicular strength (twist) of the vortex at max distance.
> ``` lang=cpp, name=Lightning
> var TwistStrengthAtMaxDistance : Real


---  
 #  TwistStrengthAtMinDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The perpendicular strength (twist) of the vortex at min distance.
> ``` lang=cpp, name=Lightning
> var TwistStrengthAtMinDistance : Real


---  
 #  VortexAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The axis the vortex spins about.
> ``` lang=cpp, name=Lightning
> var VortexAxis : Real3


---  
 #  WorldVortexAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The axis the vortex spins about in world space.
> ``` lang=cpp, name=Lightning
> var WorldVortexAxis : Real3


---  
 #  Methods


---  
 #  VortexEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function VortexEffect()
> ``` 


---  
 

 
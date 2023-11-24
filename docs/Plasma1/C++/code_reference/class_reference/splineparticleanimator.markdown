 `Component` `Gameplay`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#splineparticleanimator-v)|[ AutoCalculateLifetime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#autocalculatelifetime-ze)|[particleanimator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleanimator.markdown)| |
| |[ Helix](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#helix-plasma-engine-docume)| | |
| |[ HelixOffset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#helixoffset-plasma-engine)| | |
| |[ HelixRadius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#helixradius-plasma-engine)| | |
| |[ HelixWaveLength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#helixwavelength-plasma-eng)| | |
| |[ Mode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#mode-plasma-engine-documen)| | |
| |[ Speed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#speed-plasma-engine-docume)| | |
| |[ SpringDampingRatio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#springdampingratio-plasma)| | |
| |[ SpringFrequencyHz](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleanimator.markdown#springfrequencyhz-plasma-e)| | |


 #  Properties


---  
 #  AutoCalculateLifetime : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If checked, the lifetime on the SplineParticleEmitter will be updated to the time it would take to travel the entire path at the current speed.
> ``` lang=cpp, name=Lightning
> var AutoCalculateLifetime : Boolean


---  
 #  Helix : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Helix : Boolean


---  
 #  HelixOffset : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Offset in radians for where the helix starts.
> ``` lang=cpp, name=Lightning
> var HelixOffset : Real


---  
 #  HelixRadius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The radius of the helix.
> ``` lang=cpp, name=Lightning
> var HelixRadius : Real


---  
 #  HelixWaveLength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How fast the helix rotates in radians / second.
> ``` lang=cpp, name=Lightning
> var HelixWaveLength : Real


---  
 #  Mode : [SplineAnimatorMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#splineanimatormode)

> The current animate mode.
> ``` lang=cpp, name=Lightning
> var Mode : SplineAnimatorMode


---  
 #  Speed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The speed at which the particles move in meters / second.
> ``` lang=cpp, name=Lightning
> var Speed : Real


---  
 #  SpringDampingRatio : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var SpringDampingRatio : Real


---  
 #  SpringFrequencyHz : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Spring properties.
> ``` lang=cpp, name=Lightning
> var SpringFrequencyHz : Real


---  
 #  Methods


---  
 #  SplineParticleAnimator : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SplineParticleAnimator()
> ``` 


---  
 

 
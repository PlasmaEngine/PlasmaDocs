 `Component` `Physics`



(NOTE) Applies a directional force at the thrust effect's center. When applied to a rigid body, this will compute a torque if the force's direction does not go through the center of mass. Useful for modeling any sort of a thruster.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown#thrusteffect-void)|[ ForceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown#forcedirection-plasma-engi)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown)| |
| |[ ForceStrength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown#forcestrength-plasma-engin)| | |
| |[ LocalSpaceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown#localspacedirection-plasma)| | |
| |[ WorldForceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown#worldforcedirection-plasma)| | |


 #  Properties


---  
 #  ForceDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The direction that the force should be applied.
> ``` lang=cpp, name=Lightning
> var ForceDirection : Real3


---  
 #  ForceStrength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The strength of the force being applied in the force direction.
> ``` lang=cpp, name=Lightning
> var ForceStrength : Real


---  
 #  LocalSpaceDirection : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Determines if this force is to be applied in local or world space.
> ``` lang=cpp, name=Lightning
> var LocalSpaceDirection : Boolean


---  
 #  WorldForceDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The direction that the force should be applied in world space.
> ``` lang=cpp, name=Lightning
> var WorldForceDirection : Real3


---  
 #  Methods


---  
 #  ThrustEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ThrustEffect()
> ``` 


---  
 

 
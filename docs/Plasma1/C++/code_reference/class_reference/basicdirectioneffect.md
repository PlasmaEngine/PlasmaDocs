 `Component` `Physics`



(NOTE) Common interface for all directional force effects. Used to group together all common logic/variables for the force/gravity variants.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.md#direction-plasma-engine-do)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)|[forceeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/forceeffect.md)|
| |[ LocalSpaceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.md#localspacedirection-plasma)| |[gravityeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gravityeffect.md)|
| |[ Strength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.md#strength-plasma-engine-doc)| | |
| |[ WorldDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.md#worlddirection-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The direction that the effect will be applied in (may be in local or world space depending on the LocalSpaceDirection property).
> ``` lang=cpp, name=Lightning
> var Direction : Real3


---  
 #  LocalSpaceDirection : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the direction that the effect is applied is in local or world space. This vector is normalized when calculating forces.
> ``` lang=cpp, name=Lightning
> var LocalSpaceDirection : Boolean


---  
 #  Strength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The magnitude of the force to apply.
> ``` lang=cpp, name=Lightning
> var Strength : Real


---  
 #  WorldDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The world direction of the effect. If the effect is not in local space then this is the same as Direction.
> ``` lang=cpp, name=Lightning
> var WorldDirection : Real3


---  
 #  Methods


---  
 

 
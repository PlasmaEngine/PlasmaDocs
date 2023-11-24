 `Component` `Physics`



(NOTE) Common interface for all directional force effects. Used to group together all common logic/variables for the force/gravity variants.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.markdown#direction-plasma-engine-do)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown)|[forceeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/forceeffect.markdown)|
| |[ LocalSpaceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.markdown#localspacedirection-plasma)| |[gravityeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gravityeffect.markdown)|
| |[ Strength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.markdown#strength-plasma-engine-doc)| | |
| |[ WorldDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.markdown#worlddirection-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The direction that the effect will be applied in (may be in local or world space depending on the LocalSpaceDirection property).
> ``` lang=cpp, name=Lightning
> var Direction : Real3


---  
 #  LocalSpaceDirection : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Determines if the direction that the effect is applied is in local or world space. This vector is normalized when calculating forces.
> ``` lang=cpp, name=Lightning
> var LocalSpaceDirection : Boolean


---  
 #  Strength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The magnitude of the force to apply.
> ``` lang=cpp, name=Lightning
> var Strength : Real


---  
 #  WorldDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The world direction of the effect. If the effect is not in local space then this is the same as Direction.
> ``` lang=cpp, name=Lightning
> var WorldDirection : Real3


---  
 #  Methods


---  
 

 
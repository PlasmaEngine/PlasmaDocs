 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#particlecollisionplane-v)|[ Friction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#friction-plasma-engine-doc)|[particleanimator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleanimator.md)| |
| |[ PlaneNormal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#planenormal-plasma-engine)| | |
| |[ PlanePosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#planeposition-plasma-engin)| | |
| |[ PlaneSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#planespace-plasma-engine-d)| | |
| |[ Restitution](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlecollisionplane.md#restitution-plasma-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal. Values should be in the range [0, 1].
> ``` lang=cpp, name=Lightning
> var Friction : Real


---  
 #  PlaneNormal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var PlaneNormal : Real3


---  
 #  PlanePosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var PlanePosition : Real3


---  
 #  PlaneSpace : [SystemSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#systemspace)

> 
> ``` lang=cpp, name=Lightning
> var PlaneSpace : SystemSpace


---  
 #  Restitution : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ``` lang=cpp, name=Lightning
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionPlane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ParticleCollisionPlane()
> ``` 


---  
 

 
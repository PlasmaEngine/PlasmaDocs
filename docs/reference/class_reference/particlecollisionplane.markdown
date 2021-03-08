 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#particlecollisionplane-v)|[ Friction](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#friction-plasma-engine-doc)|[particleanimator](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particleanimator.markdown)| |
| |[ PlaneNormal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#planenormal-plasma-engine)| | |
| |[ PlanePosition](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#planeposition-plasma-engin)| | |
| |[ PlaneSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#planespace-plasma-engine-d)| | |
| |[ Restitution](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionplane.markdown#restitution-plasma-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal. Values should be in the range [0, 1].
> ``` lang=cpp, name=Lightning
> var Friction : Real


---  
 #  PlaneNormal : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var PlaneNormal : Real3


---  
 #  PlanePosition : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var PlanePosition : Real3


---  
 #  PlaneSpace : [SystemSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#systemspace)

> 
> ``` lang=cpp, name=Lightning
> var PlaneSpace : SystemSpace


---  
 #  Restitution : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
 

 
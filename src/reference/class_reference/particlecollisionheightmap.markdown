 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.markdown#particlecollisionheightm)|[ Friction](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.markdown#friction-plasma-engine-doc)|[particleanimator](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particleanimator.markdown)| |
| |[ HeightMap](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.markdown#heightmap-plasma-engine-do)| | |
| |[ Restitution](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.markdown#restitution-plasma-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal.
> ``` lang=cpp, name=Lightning
> var Friction : Real


---  
 #  HeightMap : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cogpath.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HeightMap : CogPath


---  
 #  Restitution : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ``` lang=cpp, name=Lightning
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionHeightmap : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ParticleCollisionHeightmap()
> ``` 


---  
 

 
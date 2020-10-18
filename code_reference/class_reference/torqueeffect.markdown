 `Component` `Physics`



(NOTE) Applies a torque to the center of mass of a body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/torqueeffect.markdown#torqueeffect-void)|[ LocalTorque](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/torqueeffect.markdown#localtorque-plasma-engine)|[physicseffect](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicseffect.markdown)| |
| |[ TorqueAxis](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/torqueeffect.markdown#torqueaxis-plasma-engine-d)| | |
| |[ TorqueStrength](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/torqueeffect.markdown#torquestrength-plasma-engi)| | |
| |[ WorldTorqueAxis](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/torqueeffect.markdown#worldtorqueaxis-plasma-eng)| | |


 #  Properties


---  
 #  LocalTorque : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Determines if the torque is applied in local or world space.
> ``` lang=cpp, name=Lightning
> var LocalTorque : Boolean


---  
 #  TorqueAxis : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The axis that the torque is being applied about.
> ``` lang=cpp, name=Lightning
> var TorqueAxis : Real3


---  
 #  TorqueStrength : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The strength of the torque being applied.
> ``` lang=cpp, name=Lightning
> var TorqueStrength : Real


---  
 #  WorldTorqueAxis : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The axis of the torque in world space (can be used to manually add torque to a RigidBody).
> ``` lang=cpp, name=Lightning
> var WorldTorqueAxis : Real3


---  
 #  Methods


---  
 #  TorqueEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function TorqueEffect()
> ``` 


---  
 

 
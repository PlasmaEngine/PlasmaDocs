 `Component` `Physics`



(NOTE) Applies a torque to the center of mass of a body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.md#torqueeffect-void)|[ LocalTorque](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.md#localtorque-plasma-engine)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)| |
| |[ TorqueAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.md#torqueaxis-plasma-engine-d)| | |
| |[ TorqueStrength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.md#torquestrength-plasma-engi)| | |
| |[ WorldTorqueAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.md#worldtorqueaxis-plasma-eng)| | |


 #  Properties


---  
 #  LocalTorque : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the torque is applied in local or world space.
> ``` lang=cpp, name=Lightning
> var LocalTorque : Boolean


---  
 #  TorqueAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The axis that the torque is being applied about.
> ``` lang=cpp, name=Lightning
> var TorqueAxis : Real3


---  
 #  TorqueStrength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The strength of the torque being applied.
> ``` lang=cpp, name=Lightning
> var TorqueStrength : Real


---  
 #  WorldTorqueAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

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
 

 
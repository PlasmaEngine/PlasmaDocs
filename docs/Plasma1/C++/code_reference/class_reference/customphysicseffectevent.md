 `Event` `Physics`



(NOTE) Event data for applying custom physics effects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffectevent.md#customphysicseffectevent)|[ Dt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffectevent.md#dt-plasma-engine-documenta)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ Effect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffectevent.md#effect-plasma-engine-docum)| | |
| |[ RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffectevent.md#rigidbody-plasma-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The timestep of the current physics frame (in seconds).
> ``` lang=cpp, name=Lightning
> var Dt : Real


---  
 #  Effect : [customphysicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffect.md)

> The effect that sent out this event.
> ``` lang=cpp, name=Lightning
> var Effect : CustomPhysicsEffect


---  
 #  RigidBody : [rigidbody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rigidbody.md)

> The RigidBody to apply forces to.
> ``` lang=cpp, name=Lightning
> var RigidBody : RigidBody


---  
 #  Methods


---  
 #  CustomPhysicsEffectEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CustomPhysicsEffectEvent()
> ``` 


---  
 

 
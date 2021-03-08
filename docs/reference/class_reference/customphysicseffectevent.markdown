 `Event` `Physics`



(NOTE) Event data for applying custom physics effects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/customphysicseffectevent.markdown#customphysicseffectevent)|[ Dt](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/customphysicseffectevent.markdown#dt-plasma-engine-documenta)|[event](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ Effect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/customphysicseffectevent.markdown#effect-plasma-engine-docum)| | |
| |[ RigidBody](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/customphysicseffectevent.markdown#rigidbody-plasma-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The timestep of the current physics frame (in seconds).
> ``` lang=cpp, name=Lightning
> var Dt : Real


---  
 #  Effect : [customphysicseffect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/customphysicseffect.markdown)

> The effect that sent out this event.
> ``` lang=cpp, name=Lightning
> var Effect : CustomPhysicsEffect


---  
 #  RigidBody : [rigidbody](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rigidbody.markdown)

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
 

 
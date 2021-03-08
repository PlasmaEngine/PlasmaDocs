 `Component` `Physics`



(NOTE) Defines motor properties for a joint. Used to add energy to a joint. A motor defines a desired speed to move at as well as a max impulse that can be applied to reach that speed in a timestep. See each joint for a description of how it reacts to a motor.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#jointmotor-void)|[ Active](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#active-plasma-engine-docum)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
| |[ AtomIds](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#atomids-plasma-engine-docu)| | |
| |[ MaxImpulse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#maximpulse-plasma-engine-d)| | |
| |[ Reverse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#reverse-plasma-engine-docu)| | |
| |[ Speed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointmotor.markdown#speed-plasma-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Determines if this motor is currently active.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AtomIds : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Lightning
> var AtomIds : Integer


---  
 #  MaxImpulse : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The maximum impulse that the motor can apply each frame to reach the target speed.
> ``` lang=cpp, name=Lightning
> var MaxImpulse : Real


---  
 #  Reverse : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Determines if this motor should move in reverse. This is a convenient way to reverse a motor without having to negate the speed.
> ``` lang=cpp, name=Lightning
> var Reverse : Boolean


---  
 #  Speed : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The desired speed for this motor.
> ``` lang=cpp, name=Lightning
> var Speed : Real


---  
 #  Methods


---  
 #  JointMotor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function JointMotor()
> ``` 


---  
 

 
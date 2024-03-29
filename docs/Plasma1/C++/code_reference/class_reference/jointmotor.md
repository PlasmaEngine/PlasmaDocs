 `Component` `Physics`



(NOTE) Defines motor properties for a joint. Used to add energy to a joint. A motor defines a desired speed to move at as well as a max impulse that can be applied to reach that speed in a timestep. See each joint for a description of how it reacts to a motor.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#jointmotor-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ AtomIds](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#atomids-plasma-engine-docu)| | |
| |[ MaxImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#maximpulse-plasma-engine-d)| | |
| |[ Reverse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#reverse-plasma-engine-docu)| | |
| |[ Speed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md#speed-plasma-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this motor is currently active.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AtomIds : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Lightning
> var AtomIds : Integer


---  
 #  MaxImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The maximum impulse that the motor can apply each frame to reach the target speed.
> ``` lang=cpp, name=Lightning
> var MaxImpulse : Real


---  
 #  Reverse : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this motor should move in reverse. This is a convenient way to reverse a motor without having to negate the speed.
> ``` lang=cpp, name=Lightning
> var Reverse : Boolean


---  
 #  Speed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

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
 

 
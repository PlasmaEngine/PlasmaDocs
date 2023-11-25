 `Component` `Physics`



(NOTE) A controller for a high speed physics based car. The car is controlled with a steer, gas, and brake scalar. The car will raycast wheel positions to try to keep the wheels on the ground and then apply friction and normal forces to propel the car.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ NumberOfWheelsInContact](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#numberofwheelsincontact)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#physicscar-void)|[ AntiLockBrakes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#antilockbrakes-plasma-engi)| | |
| |[ Brake](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#brake-plasma-engine-docume)| | |
| |[ DebugDraw](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#debugdraw-plasma-engine-do)| | |
| |[ Gas](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#gas-plasma-engine-document)| | |
| |[ GripScalar](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#gripscalar-plasma-engine-d)| | |
| |[ MaxSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#maxspeed-plasma-engine-doc)| | |
| |[ MaxTorque](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#maxtorque-plasma-engine-do)| | |
| |[ Steer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#steer-plasma-engine-docume)| | |
| |[ TorqueGovernor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#torquegovernor-plasma-engi)| | |
| |[ WheelCogs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#wheelcogs-plasma-engine-do)| | |
| |[ WheelFrictionFrontRollCoef](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#wheelfrictionfrontrollco)| | |
| |[ WheelFrictionSideRollCoef](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicscar.md#wheelfrictionsiderollcoe)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not the car will run any logic at all. If this is false wheels will not work, they will not behave as springs, drive, or anything else.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AntiLockBrakes : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Prevents the car from entering dynamic friction when applying brakes. If the brake would start to skid, the brake force is clamped to the max amount that will not slip.
> ``` lang=cpp, name=Lightning
> var AntiLockBrakes : Boolean


---  
 #  Brake : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the brake is being pressed [0,1] where 1 is full brake.
> ``` lang=cpp, name=Lightning
> var Brake : Real


---  
 #  DebugDraw : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not the car should debug draw.
> ``` lang=cpp, name=Lightning
> var DebugDraw : Boolean


---  
 #  Gas : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the gas is being pressed [-1,1] where -1 is full reverse.
> ``` lang=cpp, name=Lightning
> var Gas : Real


---  
 #  GripScalar : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Artificially increases the grip of the car (where 2 is twice the grip). The total grip scalar is computed as CarGripScalar * WheelGripScalar so the total car can be easily tweaked while allowing individual wheel tweaks.
> ``` lang=cpp, name=Lightning
> var GripScalar : Real


---  
 #  MaxSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The desired maximum speed of the car. Similar to a speed governor.
> ``` lang=cpp, name=Lightning
> var MaxSpeed : Real


---  
 #  MaxTorque : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The maximum torque the engine can apply to try to reach the max speed.
> ``` lang=cpp, name=Lightning
> var MaxTorque : Real


---  
 #  Steer : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the wheel is being steered. This is measured in radians about this object's y-axis.
> ``` lang=cpp, name=Lightning
> var Steer : Real


---  
 #  TorqueGovernor : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Governs the max torque that the engine can apply. This is used to keep the wheels from spinning out (slipping) when too high of a torque is applied. If the tires would slip, the engine will apply the maximum torque for the tires to not slip.
> ``` lang=cpp, name=Lightning
> var TorqueGovernor : Boolean


---  
 #  WheelCogs : [carwheelarray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/carwheelarray.md)

 `read-only`

> Read-only array of wheels belonging to this car.
> ``` lang=cpp, name=Lightning
> var WheelCogs : CarWheelArray


---  
 #  WheelFrictionFrontRollCoef : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Coefficient used to apply the forward friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ``` lang=cpp, name=Lightning
> var WheelFrictionFrontRollCoef : Real


---  
 #  WheelFrictionSideRollCoef : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Coefficient used to apply the side friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ``` lang=cpp, name=Lightning
> var WheelFrictionSideRollCoef : Real


---  
 #  Methods


---  
 #  NumberOfWheelsInContact : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of wheels currently in contact with an object.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function NumberOfWheelsInContact() : Integer
> ``` 


---  
 #  PhysicsCar : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PhysicsCar()
> ``` 


---  
 

 
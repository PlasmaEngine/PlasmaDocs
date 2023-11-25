 `Component` `Physics`



(NOTE) Controls an object's movement using joints. This allows creating a physics based character controller that reacts to physics (joints, forces, collisions, etc...). The motor controls relative velocity with respect to a target object frame.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#dynamicmotor-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ MoveInDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#moveindirection-void)|[ MaxMoveImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#maxmoveimpulse-plasma-engi)| | |
|[ SetReferenceFrameToObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#setreferenceframetoobjec)| | | |
|[ SetReferenceFrameToWorld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dynamicmotor.md#setreferenceframetoworld)| | | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should physics restrict the movement of this object?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  MaxMoveImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> What is the max impulse allowed for controlling movement.
> ``` lang=cpp, name=Lightning
> var MaxMoveImpulse : Real


---  
 #  Methods


---  
 #  DynamicMotor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DynamicMotor()
> ``` 


---  
 #  MoveInDirection : Void

> Attempts to move the body in the given direction.
> |Name|Type|Description|
> |---|---|---|
> |direction|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function MoveInDirection(direction : Real3, up : Real3)
> ``` 


---  
 #  SetReferenceFrameToObject : Void

> Compute the relative velocity with respect to a target object. Used to control movement on moving platforms.
> |Name|Type|Description|
> |---|---|---|
> |object|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function SetReferenceFrameToObject(object : Cog)
> ``` 


---  
 #  SetReferenceFrameToWorld : Void

> Compute relative velocity with respect to the world. Used to signify that an absolute world speed is desired.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SetReferenceFrameToWorld()
> ``` 


---  
 

 
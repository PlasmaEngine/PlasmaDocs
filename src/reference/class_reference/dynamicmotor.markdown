 `Component` `Physics`



(NOTE) Controls an object's movement using joints. This allows creating a physics based character controller that reacts to physics (joints, forces, collisions, etc...). The motor controls relative velocity with respect to a target object frame.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#dynamicmotor-void)|[ Active](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#active-plasma-engine-docum)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ MoveInDirection](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#moveindirection-void)|[ MaxMoveImpulse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#maxmoveimpulse-plasma-engi)| | |
|[ SetReferenceFrameToObject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#setreferenceframetoobjec)| | | |
|[ SetReferenceFrameToWorld](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dynamicmotor.markdown#setreferenceframetoworld)| | | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should physics restrict the movement of this object?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  MaxMoveImpulse : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
> |direction|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function MoveInDirection(direction : Real3, up : Real3)
> ``` 


---  
 #  SetReferenceFrameToObject : Void

> Compute the relative velocity with respect to a target object. Used to control movement on moving platforms.
> |Name|Type|Description|
> |---|---|---|
> |object|[cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)| |
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
 

 
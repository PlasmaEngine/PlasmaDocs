 `Component` `Physics`



(NOTE) Legacy. A linear axis joint is used to keep an object locked on a plane that is defined by a normal. This was made to help make a dynamic character controller. Instead of locking translation along a plane, the constraint can be turned off with a motor attached to it which will drive movement in the direction of the plane normal. This can then be thought of as a "move in direction" constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearaxisjoint.md#linearaxisjoint-void)|[ WorldAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearaxisjoint.md#worldaxis-plasma-engine-do)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |


 #  Properties


---  
 #  WorldAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The axis in world space that is constrained.
> ``` lang=cpp, name=Lightning
> var WorldAxis : Real3


---  
 #  Methods


---  
 #  LinearAxisJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function LinearAxisJoint()
> ``` 


---  
 

 
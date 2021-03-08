 `Component` `Physics`



(NOTE) A joint that models a wheel with shocks. A wheel aligns the two local axes together and allows free rotation about this axis. The specified shock axis is turned into a soft constraint to model the shocks. Note: ObjectA should be the root object as the shock axis rotates with this object. If ObjectA is the wheel, then the shock axis will rotate with the wheel, causing the shocks to not stay aligned. Add on definitions: Limit: A limit will provide a min/max angle on the motor axis. Motor: A motor will turn the objects about the motor axis. Spring: A spring will make the shock axis springy. A spring is attached by default to a wheel.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#setworldpoints-void)|[ LocalAxisA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localaxisa-plasma-engine-d)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#wheeljoint-void)|[ LocalAxisB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localaxisb-plasma-engine-d)| | |
| |[ LocalBasisA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localbasisa-plasma-engine)| | |
| |[ LocalBasisB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localbasisb-plasma-engine)| | |
| |[ LocalPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#localpointb-plasma-engine)| | |
| |[ ShockAxis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#shockaxis-plasma-engine-do)| | |
| |[ WorldAxis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#worldaxis-plasma-engine-do)| | |
| |[ WorldPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#worldpointb-plasma-engine)| | |
| |[ WorldShockAxis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/wheeljoint.markdown#worldshockaxis-plasma-engi)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object A . 
> ``` lang=cpp, name=Lightning
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object B . 
> ``` lang=cpp, name=Lightning
> var LocalAxisB : Real3


---  
 #  LocalBasisA : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> The local space reference frame of object A . This frame is transformed to world space and then aligned with object B s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisA : Quaternion


---  
 #  LocalBasisB : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> The local space reference frame of object B . This frame is transformed to world space and then aligned with object A s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisB : Quaternion


---  
 #  LocalPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The local point of the anchor on object A . 
> ``` lang=cpp, name=Lightning
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The local point of the anchor on object B . 
> ``` lang=cpp, name=Lightning
> var LocalPointB : Real3


---  
 #  ShockAxis : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The shock axis in the local space of body A.
> ``` lang=cpp, name=Lightning
> var ShockAxis : Real3


---  
 #  WorldAxis : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The axis in world space that is being rotated about . 
> ``` lang=cpp, name=Lightning
> var WorldAxis : Real3


---  
 #  WorldPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The position of the anchor on object A given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The position of the anchor on object B given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointB : Real3


---  
 #  WorldShockAxis : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The shock axis after it has been translated into world space.
> ``` lang=cpp, name=Lightning
> var WorldShockAxis : Real3


---  
 #  Methods


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetWorldPoints(point : Real3)
> ``` 


---  
 #  WheelJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WheelJoint()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) A revolute joint is used to create a wheel or a hinge. A revolute joint bring the two locally defined axes together and allows free rotation only on that axis. This axis is also where the motor is applied. The two axes that are orthogonal to the motor axis have their rotation locked (objects rotate together unless on the motor axis). Add on definitions: Limit: A limit will provide a min/max angle on the motor axis. Zero is defined by the location of the primary axis on the FrameOfreference object. Motor: A motor will drive the objects about the motor axis. Spring: A spring will make the motor axis springy at the limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#revolutejoint-void)|[ FrameOfReference](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#frameofreference-plasma-en)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)| |
|[ SetWorldFrame](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#setworldframe-void)|[ LocalBasisA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#localbasisa-plasma-engine)| | |
|[ SetWorldPoints](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#setworldpoints-void)|[ LocalBasisB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#localbasisb-plasma-engine)| | |
| |[ LocalPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#localpointb-plasma-engine)| | |
| |[ WorldBasis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#worldbasis-plasma-engine-d)| | |
| |[ WorldPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/revolutejoint.markdown#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  FrameOfReference : [JointFrameOfReference](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#jointframeofreference)

> Should the default basis of the constraint be object A or B? This determines which object's world axis is used when constructing the basis for the constraint. In the case of a dynamic and static object, the static object is generally the better choice. As a general rule of thumb, it should be the heavier/most important object.
> ``` lang=cpp, name=Lightning
> var FrameOfReference : JointFrameOfReference


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
 #  WorldBasis : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> The basis of the joint in world-space. This basis will come object specified by FrameOfReference. The basis is constructed such that the x-axis is the primary axis while the z-axis is the hinge axis.
> ``` lang=cpp, name=Lightning
> var WorldBasis : Quaternion


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
 #  Methods


---  
 #  RevoluteJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RevoluteJoint()
> ``` 


---  
 #  SetWorldFrame : Void

> Legacy. Used to set the entire frame in world space for this joint. The x and y axes are used as a basis for limiting the joint. The x axis is at angle 0 and the y axis is at angle 90. The z axis is the axis of rotational freedom.
> |Name|Type|Description|
> |---|---|---|
> |rot|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetWorldFrame(rot : Quaternion)
> ``` 


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
 

 
 `Component` `Physics`



(NOTE) A prismatic joint sometimes called a slider) is used to create something similar to a piston. This joint fixes all degrees of rotation and leaves one linear axis free. Therefore, the bodies will rotate with each other and move with each other, except for one axis where they can move freely. Add on definitions: Limit: A limit will provide a min/max translational distance for the two objects on the slider axis. Motor: A motor will push/pull the objects on the slider axis. Spring: A spring will make the slider axis springy at its limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#prismaticjoint-void)|[ LocalAxisA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localaxisa-plasma-engine-d)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)| |
|[ SetWorldPoints](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#setworldpoints-void)|[ LocalAxisB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localaxisb-plasma-engine-d)| | |
| |[ LocalBasisA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localbasisa-plasma-engine)| | |
| |[ LocalBasisB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localbasisb-plasma-engine)| | |
| |[ LocalPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#localpointb-plasma-engine)| | |
| |[ WorldAxis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#worldaxis-plasma-engine-do)| | |
| |[ WorldPointA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/prismaticjoint.markdown#worldpointb-plasma-engine)| | |


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
 #  Methods


---  
 #  PrismaticJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PrismaticJoint()
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
 

 
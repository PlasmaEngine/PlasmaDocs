 `Component` `Physics`



(NOTE) A prismatic joint is used to create something similar to a piston. This is the 2d version of PrismaticJoint. This joint is used in 2d mode for increased performance and stability. The slider axis is projected onto the z axis (the z component is ignored) so that the objects can be arbitrarily far apart. The x and y rotations are also ignored since the objects are only allowed to rotate about the z axis. Add on definitions: Limit: A limit will provide a min/max translational distance for the two objects on the slider axis. Motor: A motor will push/pull the objects on the slider axis. Spring: A spring will make the slider axis springy at its limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#prismaticjoint2d-void)|[ LocalAxisA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localaxisa-plasma-engine-d)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
|[ SetWorldPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#setworldpoints-void)|[ LocalAxisB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localaxisb-plasma-engine-d)| | |
| |[ LocalBasisA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localbasisa-plasma-engine)| | |
| |[ LocalBasisB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localbasisb-plasma-engine)| | |
| |[ LocalPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#localpointb-plasma-engine)| | |
| |[ WorldAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#worldaxis-plasma-engine-do)| | |
| |[ WorldPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The locally defined axis on object A . 
> ``` lang=cpp, name=Lightning
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The locally defined axis on object B . 
> ``` lang=cpp, name=Lightning
> var LocalAxisB : Real3


---  
 #  LocalBasisA : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> The local space reference frame of object A . This frame is transformed to world space and then aligned with object B s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisA : Quaternion


---  
 #  LocalBasisB : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> The local space reference frame of object B . This frame is transformed to world space and then aligned with object A s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisB : Quaternion


---  
 #  LocalPointA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The local point of the anchor on object A . 
> ``` lang=cpp, name=Lightning
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The local point of the anchor on object B . 
> ``` lang=cpp, name=Lightning
> var LocalPointB : Real3


---  
 #  WorldAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The axis in world space that is being rotated about . 
> ``` lang=cpp, name=Lightning
> var WorldAxis : Real3


---  
 #  WorldPointA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  PrismaticJoint2d : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PrismaticJoint2d()
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
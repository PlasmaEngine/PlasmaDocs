 `Component` `Physics`



(NOTE) A weld joint is used to lock the position and orientation of two objects together. Welds should generally not be used to make two objects rigid as they are computationally more expensive and less rigid than using composites. The primary uses for welds are for quick connections or connections that are desired to not be fully rigid. Also, while it can be done with composites too, welds can be used to model object breaking beyond some max force. Limits, motors and springs should most likely not be used on this. Add on definitions: Limit: A limit will provide a min/max translation on the x, y, and z axes. Motor: A motor will attempt to drive the rotation on the x, y, and z axes. Spring: A spring will make the x, y, and z axis springy.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#setworldpoints-void)|[ LocalBasisA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#localbasisa-plasma-engine)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/joint.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#weldjoint-void)|[ LocalBasisB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#localbasisb-plasma-engine)| | |
| |[ LocalPointA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#localpointb-plasma-engine)| | |
| |[ WorldPointA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/weldjoint.markdown#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  LocalBasisA : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/quaternion.markdown)

> The local space reference frame of object A . This frame is transformed to world space and then aligned with object B s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisA : Quaternion


---  
 #  LocalBasisB : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/quaternion.markdown)

> The local space reference frame of object B . This frame is transformed to world space and then aligned with object A s frame . 
> ``` lang=cpp, name=Lightning
> var LocalBasisB : Quaternion


---  
 #  LocalPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The local point of the anchor on object A . 
> ``` lang=cpp, name=Lightning
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The local point of the anchor on object B . 
> ``` lang=cpp, name=Lightning
> var LocalPointB : Real3


---  
 #  WorldPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The position of the anchor on object A given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The position of the anchor on object B given a position in world space 
> ``` lang=cpp, name=Lightning
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetWorldPoints(point : Real3)
> ``` 


---  
 #  WeldJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WeldJoint()
> ``` 


---  
 

 
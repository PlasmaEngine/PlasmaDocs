 `Component` `Physics`



(NOTE) Represents a ball and socket joint. A position joint constrains the two anchor points on each object to be equal. Limits, motors, and springs typically should not be used. Add on definitions: Limit: A limit will provide a min/max translation on every axis (x,y,z) that the objects must be between. Motor: A motor will attempt to drive the translation in the positive direction on every axis. Spring: A spring will make the translation on every axis springy at the bounds.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#positionjoint-void)|[ LocalPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#localpointa-plasma-engine)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
|[ SetWorldPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#setworldpoints-void)|[ LocalPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#localpointb-plasma-engine)| | |
| |[ WorldPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md#worldpointb-plasma-engine)| | |


 #  Properties


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
 #  PositionJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PositionJoint()
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
 

 
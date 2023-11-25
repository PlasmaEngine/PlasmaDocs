 `Component` `Physics`



(NOTE) A universal joint locks positional movement of two points together as well as locking rotation about one axis. This means it is a joint that constrains four axes and leaves two free rotational axes. This joint is most useful to model something like a arm or leg that has a large range of rotational movement.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#setworldpoints-void)|[ LocalAxis0OfBodyA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localaxis0ofbodya-plasma-e)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#universaljoint-void)|[ LocalAxis0OfBodyB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localaxis0ofbodyb-plasma-e)| | |
| |[ LocalAxis1OfBodyA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localaxis1ofbodya-plasma-e)| | |
| |[ LocalAxis1OfBodyB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localaxis1ofbodyb-plasma-e)| | |
| |[ LocalPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localpointa-plasma-engine)| | |
| |[ LocalPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#localpointb-plasma-engine)| | |
| |[ WorldPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  LocalAxis0OfBodyA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ``` lang=cpp, name=Lightning
> var LocalAxis0OfBodyA : Real3


---  
 #  LocalAxis0OfBodyB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ``` lang=cpp, name=Lightning
> var LocalAxis0OfBodyB : Real3


---  
 #  LocalAxis1OfBodyA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ``` lang=cpp, name=Lightning
> var LocalAxis1OfBodyA : Real3


---  
 #  LocalAxis1OfBodyB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ``` lang=cpp, name=Lightning
> var LocalAxis1OfBodyB : Real3


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
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function SetWorldPoints(point : Real3)
> ``` 


---  
 #  UniversalJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UniversalJoint()
> ``` 


---  
 

 
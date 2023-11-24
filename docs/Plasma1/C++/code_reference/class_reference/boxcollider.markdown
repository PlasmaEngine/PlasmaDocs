 `Component` `Physics`



(NOTE) Defines the collision volume of a box defined by a size on each axis.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.markdown#boxcollider-void)|[ HalfSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.markdown#halfsize-plasma-engine-doc)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)| |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.markdown#size-plasma-engine-documen)| | |
| |[ WorldSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.markdown#worldsize-plasma-engine-do)| | |


 #  Properties


---  
 #  HalfSize : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The half size (from the center to the upper-right corner) on each axis of the box in local space. Used to make the box's size match a model or some other volume without needing to scale the transform (also avoids non-uniform scale issues).
> ``` lang=cpp, name=Lightning
> var HalfSize : Real3


---  
 #  Size : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The size (from min to max) on each axis of the box in local space. Used to make the box's size match a model or some other volume without needing to scale the transform (also avoids non-uniform scale issues).
> ``` lang=cpp, name=Lightning
> var Size : Real3


---  
 #  WorldSize : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The size of the box after the transform is applied (scale and rotation).
> ``` lang=cpp, name=Lightning
> var WorldSize : Real3


---  
 #  Methods


---  
 #  BoxCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function BoxCollider()
> ``` 


---  
 

 
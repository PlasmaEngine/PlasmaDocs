 `Component` `Physics`



(NOTE) Defines the collision volume for a cylinder defined by a height and radius.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#cylindercollider-void)|[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#direction-plasma-engine-do)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
| |[ Height](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#height-plasma-engine-docum)| | |
| |[ Radius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#radius-plasma-engine-docum)| | |
| |[ WorldHeight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#worldheight-plasma-engine)| | |
| |[ WorldRadius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md#worldradius-plasma-engine)| | |


 #  Properties


---  
 #  Direction : [AxisDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#axisdirection)

> The direction that the height is defined along. Allows the user to change whether the cylinder's height is along the x, y, or z axis.
> ``` lang=cpp, name=Lightning
> var Direction : AxisDirection


---  
 #  Height : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The local space distance from the top of the cylinder to the bottom.
> ``` lang=cpp, name=Lightning
> var Height : Real


---  
 #  Radius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The local space radius of the cylinder.
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  WorldHeight : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The full height of the cylinder after scale is applied.
> ``` lang=cpp, name=Lightning
> var WorldHeight : Real


---  
 #  WorldRadius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The radius of the cylinder after scale is applied.
> ``` lang=cpp, name=Lightning
> var WorldRadius : Real


---  
 #  Methods


---  
 #  CylinderCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CylinderCollider()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) Defines the collision volume for a capsule defined by a height and radius. A capsule can be thought of as a cylinder with spherical end caps.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#capsulecollider-void)|[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#direction-plasma-engine-do)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
| |[ Height](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#height-plasma-engine-docum)| | |
| |[ Radius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#radius-plasma-engine-docum)| | |
| |[ ScalingMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#scalingmode-plasma-engine)| | |
| |[ WorldCylinderHeight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#worldcylinderheight-plasma)| | |
| |[ WorldRadius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md#worldradius-plasma-engine)| | |


 #  Properties


---  
 #  Direction : [AxisDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#axisdirection)

> The direction that the height is defined along. Allows the user to change whether the capsule's height is along the local-space x, y, or z axis.
> ``` lang=cpp, name=Lightning
> var Direction : AxisDirection


---  
 #  Height : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The local space distance from the center of one sphere to another.
> ``` lang=cpp, name=Lightning
> var Height : Real


---  
 #  Radius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The local space radius of the spheres at the capsule edges.
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  ScalingMode : [CapsuleScalingMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#capsulescalingmode)

> How should non-uniform scale affect the capsules size. Should a scale of 2 on the height axis double the total capsule size or should it double the capsule height?
> ``` lang=cpp, name=Lightning
> var ScalingMode : CapsuleScalingMode


---  
 #  WorldCylinderHeight : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The full height of the capsule's cylinder after the scale is applied (world distance from one sphere to another).
> ``` lang=cpp, name=Lightning
> var WorldCylinderHeight : Real


---  
 #  WorldRadius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The radius of the sphere caps after scale is applied.
> ``` lang=cpp, name=Lightning
> var WorldRadius : Real


---  
 #  Methods


---  
 #  CapsuleCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CapsuleCollider()
> ``` 


---  
 

 
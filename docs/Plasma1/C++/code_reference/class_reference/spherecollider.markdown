 `Component` `Physics`



(NOTE) Defines the collision volume for a sphere defined by a radius.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spherecollider.markdown#spherecollider-void)|[ Radius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spherecollider.markdown#radius-plasma-engine-docum)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)| |
| |[ WorldRadius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spherecollider.markdown#worldradius-plasma-engine)| | |


 #  Properties


---  
 #  Radius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The radius of the sphere in local space (before transform is applied).
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  WorldRadius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The radius of the sphere after transform is applied (scale).
> ``` lang=cpp, name=Lightning
> var WorldRadius : Real


---  
 #  Methods


---  
 #  SphereCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SphereCollider()
> ``` 


---  
 

 
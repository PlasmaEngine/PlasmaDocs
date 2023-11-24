 `Component` `Physics`



(NOTE) Defines the collision volume for an ellipsoid (3 dimensional ellipse) defined by three radius values.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ellipsoidcollider.markdown#ellipsoidcollider-void)|[ Radii](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ellipsoidcollider.markdown#radii-plasma-engine-docume)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)| |
| |[ WorldRadii](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ellipsoidcollider.markdown#worldradii-plasma-engine-d)| | |


 #  Properties


---  
 #  Radii : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The x, y, and z radius of the ellipsoid.
> ``` lang=cpp, name=Lightning
> var Radii : Real3


---  
 #  WorldRadii : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The radii of the ellipsoid after transform is applied (scale and rotation).
> ``` lang=cpp, name=Lightning
> var WorldRadii : Real3


---  
 #  Methods


---  
 #  EllipsoidCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function EllipsoidCollider()
> ``` 


---  
 

 
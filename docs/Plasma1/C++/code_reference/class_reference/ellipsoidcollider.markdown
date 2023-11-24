 `Component` `Physics`



(NOTE) Defines the collision volume for an ellipsoid (3 dimensional ellipse) defined by three radius values.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ellipsoidcollider.markdown#ellipsoidcollider-void)|[ Radii](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ellipsoidcollider.markdown#radii-plasma-engine-docume)|[collider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/collider.markdown)| |
| |[ WorldRadii](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ellipsoidcollider.markdown#worldradii-plasma-engine-d)| | |


 #  Properties


---  
 #  Radii : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The x, y, and z radius of the ellipsoid.
> ``` lang=cpp, name=Lightning
> var Radii : Real3


---  
 #  WorldRadii : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

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
 

 
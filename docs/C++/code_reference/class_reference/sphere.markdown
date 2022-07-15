 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Expand](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#expand-void)|[ Center](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#center-plasma-engine-docum)| | |
|[ Overlap](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#overlap-plasma-engine-docu)|[ Radius](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#radius-plasma-engine-docum)| | |
|[ Overlaps](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#overlaps-plasma-engine-doc)|[ SurfaceArea](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#surfacearea-plasma-engine)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#sphere-void)|[ Volume](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  Center : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Center : Real3


---  
 #  Radius : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  SurfaceArea : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var SurfaceArea : Real


---  
 #  Volume : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  Methods


---  
 #  Expand : Void

> Expand this sphere to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Real3)
> ``` 


---  
 #  Expand : [sphere](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown)

 `static`

> Creates a sphere that contains the given sphere and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown)| |
> |p1|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Sphere, p1 : Real3) : Sphere
> ``` 


---  
 #  Overlap : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown)| |
> ``` lang=cpp, name=Lightning
> function Overlap(p0 : Sphere) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Does this sphere overlap/intersect the given sphere?
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown)| |
> ``` lang=cpp, name=Lightning
> function Overlaps(p0 : Sphere) : Boolean
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Sphere()
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |radius|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Sphere(center : Real3, radius : Real)
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sphere.markdown)| |
> ``` lang=cpp, name=Lightning
> function Sphere(p0 : Sphere)
> ``` 


---  
 

 
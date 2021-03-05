 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#aabb-void)|[ Center](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#center-plasma-engine-docum)| | |
|[ ContainsPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#containspoint-plasma-engin)|[ Extents](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#extents-plasma-engine-docu)| | |
|[ Expand](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#expand-void)|[ HalfExtents](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#halfextents-plasma-engine)| | |
|[ Overlap](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#overlap-plasma-engine-docu)|[ Max](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#max-plasma-engine-document)| | |
|[ Overlaps](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#overlaps-plasma-engine-doc)|[ Min](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#min-plasma-engine-document)| | |
|[ Set](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#set-void)|[ SurfaceArea](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#surfacearea-plasma-engine)| | |
|[ SetInvalid](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#setinvalid-void)|[ Volume](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#volume-plasma-engine-docum)| | |
|[ ZeroOut](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown#plasmaout-void)| | | |


 #  Properties


---  
 #  Center : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Center : Real3


---  
 #  Extents : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Extents : Real3


---  
 #  HalfExtents : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HalfExtents : Real3


---  
 #  Max : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Max : Real3


---  
 #  Min : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Min : Real3


---  
 #  SurfaceArea : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var SurfaceArea : Real


---  
 #  Volume : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  Methods


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Aabb()
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function Aabb(p0 : Aabb)
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Aabb(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  ContainsPoint : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Does this aabb contain the given point?
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function ContainsPoint(p0 : Real3) : Boolean
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given aabb.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb)
> ``` 


---  
 #  Expand : [aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)

 `static`

> Creates an aabb that contains the two given aabbs.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> |p1|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb, p1 : Aabb) : Aabb
> ``` 


---  
 #  Expand : [aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)

 `static`

> Creates an aabb that contains the given aabb and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> |p1|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb, p1 : Real3) : Aabb
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Real3)
> ``` 


---  
 #  Overlap : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function Overlap(p0 : Aabb) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Does this aabb overlap/intersect the given aabb?
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function Overlaps(p0 : Aabb) : Boolean
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  SetInvalid : Void

> Sets this aabb to an invalid aabb (Real3.PositiveMax, Real3.NegativeMin)). This also makes expansion easier.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SetInvalid()
> ``` 


---  
 #  ZeroOut : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ZeroOut()
> ``` 


---  
 

 
 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#aabb-void)|[ Center](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#center-plasma-engine-docum)| | |
|[ ContainsPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#containspoint-plasma-engin)|[ Extents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#extents-plasma-engine-docu)| | |
|[ Expand](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#expand-void)|[ HalfExtents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#halfextents-plasma-engine)| | |
|[ Overlap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#overlap-plasma-engine-docu)|[ Max](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#max-plasma-engine-document)| | |
|[ Overlaps](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#overlaps-plasma-engine-doc)|[ Min](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#min-plasma-engine-document)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#set-void)|[ SurfaceArea](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#surfacearea-plasma-engine)| | |
|[ SetInvalid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#setinvalid-void)|[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#volume-plasma-engine-docum)| | |
|[ ZeroOut](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md#plasmaout-void)| | | |


 #  Properties


---  
 #  Center : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Center : Real3


---  
 #  Extents : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Extents : Real3


---  
 #  HalfExtents : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var HalfExtents : Real3


---  
 #  Max : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Max : Real3


---  
 #  Min : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Min : Real3


---  
 #  SurfaceArea : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var SurfaceArea : Real


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

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
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Lightning
> function Aabb(p0 : Aabb)
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |halfExtents|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Aabb(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  ContainsPoint : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Does this aabb contain the given point?
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function ContainsPoint(p0 : Real3) : Boolean
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given aabb.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb)
> ``` 


---  
 #  Expand : [aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)

 `static`

> Creates an aabb that contains the two given aabbs.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> |p1|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb, p1 : Aabb) : Aabb
> ``` 


---  
 #  Expand : [aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)

 `static`

> Creates an aabb that contains the given aabb and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> |p1|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Aabb, p1 : Real3) : Aabb
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Expand(p0 : Real3)
> ``` 


---  
 #  Overlap : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Lightning
> function Overlap(p0 : Aabb) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Does this aabb overlap/intersect the given aabb?
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Lightning
> function Overlaps(p0 : Aabb) : Boolean
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Set(point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |halfExtents|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
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
 

 
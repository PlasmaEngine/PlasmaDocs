 `Physics`

(NOTE) A result from a cast operation on a PhysicsSpace.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#castresult-void)|[ Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#collider-plasma-engine-doc)| | |
|[ GetLocalPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#getlocalposition-plasma-en)|[ Distance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#distance-plasma-engine-doc)| | |
| |[ Normal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#normal-plasma-engine-docum)| | |
| |[ ObjectHit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#objecthit-plasma-engine-do)| | |
| |[ WorldPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md#worldposition-plasma-engin)| | |


 #  Properties


---  
 #  Collider : [collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)

 `read-only`

> The collider hit by the cast.
> ``` lang=cpp, name=Lightning
> var Collider : Collider


---  
 #  Distance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The distance from the ray/segment start to the point of intersection. Invalid on a volume cast.
> ``` lang=cpp, name=Lightning
> var Distance : Real


---  
 #  Normal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The normal of the object at the intersection point (world space). Invalid on a volume cast.
> ``` lang=cpp, name=Lightning
> var Normal : Real3


---  
 #  ObjectHit : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The cog hit by the cast.
> ``` lang=cpp, name=Lightning
> var ObjectHit : Cog


---  
 #  WorldPosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> Returns the world-space position that the object was hit. Invalid on a volume cast.
> ``` lang=cpp, name=Lightning
> var WorldPosition : Real3


---  
 #  Methods


---  
 #  CastResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CastResult()
> ``` 


---  
 #  CastResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |rhs|[castresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md)| |
> ``` lang=cpp, name=Lightning
> function CastResult(rhs : CastResult)
> ``` 


---  
 #  GetLocalPosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Returns the local-space position that the object was hit. The point index is used to get the first or last point of intersection. Invalid on volume casts.
> |Name|Type|Description|
> |---|---|---|
> |pointIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetLocalPosition(pointIndex : Integer) : Real3
> ``` 


---  
 

 
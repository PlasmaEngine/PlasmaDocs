 `Physics`

(NOTE) A result from a cast operation on a PhysicsSpace.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#castresult-void)|[ Collider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#collider-plasma-engine-doc)| | |
|[ GetLocalPosition](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#getlocalposition-plasma-en)|[ Distance](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#distance-plasma-engine-doc)| | |
| |[ Normal](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#normal-plasma-engine-docum)| | |
| |[ ObjectHit](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#objecthit-plasma-engine-do)| | |
| |[ WorldPosition](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown#worldposition-plasma-engin)| | |


 #  Properties


---  
 #  Collider : [collider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown)

 `read-only`

> The collider hit by the cast.
> ``` lang=cpp, name=Lightning
> var Collider : Collider


---  
 #  Distance : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The distance from the ray/segment start to the point of intersection. Invalid on a volume cast.
> ``` lang=cpp, name=Lightning
> var Distance : Real


---  
 #  Normal : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The normal of the object at the intersection point (world space). Invalid on a volume cast.
> ``` lang=cpp, name=Lightning
> var Normal : Real3


---  
 #  ObjectHit : [cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> The cog hit by the cast.
> ``` lang=cpp, name=Lightning
> var ObjectHit : Cog


---  
 #  WorldPosition : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

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
> |rhs|[castresult](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/castresult.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastResult(rhs : CastResult)
> ``` 


---  
 #  GetLocalPosition : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Returns the local-space position that the object was hit. The point index is used to get the first or last point of intersection. Invalid on volume casts.
> |Name|Type|Description|
> |---|---|---|
> |pointIndex|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetLocalPosition(pointIndex : Integer) : Real3
> ``` 


---  
 

 
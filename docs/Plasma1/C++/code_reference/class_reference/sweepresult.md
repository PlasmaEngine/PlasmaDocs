 `Physics`

(NOTE) Cast result from performing a sweep test.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#sweepresult-void)|[ OtherCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#othercollider-plasma-engin)| | |
| |[ OtherObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#otherobject-plasma-engine)| | |
| |[ Penetration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#penetration-plasma-engine)| | |
| |[ Time](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#time-plasma-engine-documen)| | |
| |[ WorldNormalTowardsOther](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#worldnormaltowardsother)| | |
| |[ WorldNormalTowardsSelf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#worldnormaltowardsself-z)| | |
| |[ WorldPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md#worldpoint-plasma-engine-d)| | |


 #  Properties


---  
 #  OtherCollider : [collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)

 `read-only`

> The other collider being hit.
> ``` lang=cpp, name=Lightning
> var OtherCollider : Collider


---  
 #  OtherObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The other cog being hit.
> ``` lang=cpp, name=Lightning
> var OtherObject : Cog


---  
 #  Penetration : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The amount of overlap with this object. Will typically be plasma unless the objects start in contact.
> ``` lang=cpp, name=Lightning
> var Penetration : Real


---  
 #  Time : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The time of impact that this collision first happens.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  WorldNormalTowardsOther : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The contact normal pointing from the sweeping object towards the other object.
> ``` lang=cpp, name=Lightning
> var WorldNormalTowardsOther : Real3


---  
 #  WorldNormalTowardsSelf : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The contact normal pointing from the other object towards the sweeping object.
> ``` lang=cpp, name=Lightning
> var WorldNormalTowardsSelf : Real3


---  
 #  WorldPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The point of intersection in world-space.
> ``` lang=cpp, name=Lightning
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SweepResult()
> ``` 


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[sweepresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.md)| |
> ``` lang=cpp, name=Lightning
> function SweepResult( : SweepResult)
> ``` 


---  
 

 
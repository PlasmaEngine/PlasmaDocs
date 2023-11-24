 `Physics`

(NOTE) Cast result from performing a sweep test.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#sweepresult-void)|[ OtherCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#othercollider-plasma-engin)| | |
| |[ OtherObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#otherobject-plasma-engine)| | |
| |[ Penetration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#penetration-plasma-engine)| | |
| |[ Time](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#time-plasma-engine-documen)| | |
| |[ WorldNormalTowardsOther](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#worldnormaltowardsother)| | |
| |[ WorldNormalTowardsSelf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#worldnormaltowardsself-z)| | |
| |[ WorldPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown#worldpoint-plasma-engine-d)| | |


 #  Properties


---  
 #  OtherCollider : [collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)

 `read-only`

> The other collider being hit.
> ``` lang=cpp, name=Lightning
> var OtherCollider : Collider


---  
 #  OtherObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The other cog being hit.
> ``` lang=cpp, name=Lightning
> var OtherObject : Cog


---  
 #  Penetration : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The amount of overlap with this object. Will typically be plasma unless the objects start in contact.
> ``` lang=cpp, name=Lightning
> var Penetration : Real


---  
 #  Time : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The time of impact that this collision first happens.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  WorldNormalTowardsOther : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The contact normal pointing from the sweeping object towards the other object.
> ``` lang=cpp, name=Lightning
> var WorldNormalTowardsOther : Real3


---  
 #  WorldNormalTowardsSelf : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The contact normal pointing from the other object towards the sweeping object.
> ``` lang=cpp, name=Lightning
> var WorldNormalTowardsSelf : Real3


---  
 #  WorldPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

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
> ||[sweepresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresult.markdown)| |
> ``` lang=cpp, name=Lightning
> function SweepResult( : SweepResult)
> ``` 


---  
 

 
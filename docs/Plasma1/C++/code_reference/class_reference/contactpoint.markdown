 `Physics`



(NOTE) Information about one point of contact in a collision. This is useful for evaluating info about the collision after it happened such as where the objects hit. WARNING: Do not hold onto this after an event is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#contactpoint-void)|[ ComplexImpulse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#compleximpulse-plasma-engi)| | |
| |[ FrictionImpulse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#frictionimpulse-plasma-eng)| | |
| |[ LocalPoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#localpoint-plasma-engine-d)| | |
| |[ NormalImpulse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#normalimpulse-plasma-engin)| | |
| |[ OtherLocalPoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#otherlocalpoint-plasma-eng)| | |
| |[ Penetration](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#penetration-plasma-engine)| | |
| |[ RelativeVelocity](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#relativevelocity-plasma-en)| | |
| |[ WorldNormalTowardsOther](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#worldnormaltowardsother)| | |
| |[ WorldPoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown#worldpoint-plasma-engine-d)| | |


 #  Properties


---  
 #  ComplexImpulse : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The total impulse this object applied (only for more complicated logic). The impulse is a Vector3 of the values (normal, friction1, friction2).
> ``` lang=cpp, name=Lightning
> var ComplexImpulse : Real3


---  
 #  FrictionImpulse : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The total friction impulse that this object applied.
> ``` lang=cpp, name=Lightning
> var FrictionImpulse : Real


---  
 #  LocalPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The point in local space of myself in this collision.
> ``` lang=cpp, name=Lightning
> var LocalPoint : Real3


---  
 #  NormalImpulse : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The total impulse that this object applied in the direction of the normal.
> ``` lang=cpp, name=Lightning
> var NormalImpulse : Real


---  
 #  OtherLocalPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The point in local space of the other object in this collision.
> ``` lang=cpp, name=Lightning
> var OtherLocalPoint : Real3


---  
 #  Penetration : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The penetration of this contact point in the direction of the normal. Note: penetration is always positive and is not flipped for object A or object B.
> ``` lang=cpp, name=Lightning
> var Penetration : Real


---  
 #  RelativeVelocity : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The relative velocity of this point in the direction of the normal. The relative point velocity is defined as Dot(p1 - p0, n) where p1 and p0 are the velocities of the contact points in the collision of myself and the other object respectively. This value can be used to see how fast the objects are now separating. Also, in pre-collision this value can be used to approximate the impulse of the collision since the impulse values will not have been calculated yet in pre-collision.
> ``` lang=cpp, name=Lightning
> var RelativeVelocity : Real


---  
 #  WorldNormalTowardsOther : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The world space normal that points from myself towards the other object.
> ``` lang=cpp, name=Lightning
> var WorldNormalTowardsOther : Real3


---  
 #  WorldPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The point in world space of this contact point.
> ``` lang=cpp, name=Lightning
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  ContactPoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ContactPoint()
> ``` 


---  
 #  ContactPoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[contactpoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown)| |
> ``` lang=cpp, name=Lightning
> function ContactPoint( : ContactPoint)
> ``` 


---  
 

 
 `Event` `Physics`



(NOTE) Common interface for all collision events. Contains shared methods to access contact information for a collision.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ContactPointCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basecollisionevent.markdown#contactpointcount-plasma-e)|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)|[collisionevent](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collisionevent.markdown)|
| |[ ContactPoints](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basecollisionevent.markdown#contactpoints-plasma-engin)| |[collisiongroupevent](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroupevent.markdown)|
| |[ IsGhost](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basecollisionevent.markdown#isghost-plasma-engine-docu)| |[presolveevent](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/presolveevent.markdown)|
| |[ Object](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basecollisionevent.markdown#object-plasma-engine-docum)| | |
| |[ OtherObject](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basecollisionevent.markdown#otherobject-plasma-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> The number of contact points in this collision.
> ``` lang=cpp, name=Lightning
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/contactpointrange.markdown)

 `read-only`

> A range for iterating through all contact points.
> ``` lang=cpp, name=Lightning
> var ContactPoints : ContactPointRange


---  
 #  IsGhost : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> If this was a ghost collision (detected but not resolved).
> ``` lang=cpp, name=Lightning
> var IsGhost : Boolean


---  
 #  Object : [cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> The object that this event was sent to.
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  OtherObject : [cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> The other object in this collision.
> ``` lang=cpp, name=Lightning
> var OtherObject : Cog


---  
 #  Methods


---  
 

 
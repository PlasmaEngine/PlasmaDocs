 `Event` `Physics`



(NOTE) Common interface for all collision events. Contains shared methods to access contact information for a collision.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ContactPointCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md#contactpointcount-plasma-e)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)|[collisionevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionevent.md)|
| |[ ContactPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md#contactpoints-plasma-engin)| |[collisiongroupevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.md)|
| |[ IsGhost](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md#isghost-plasma-engine-docu)| |[presolveevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/presolveevent.md)|
| |[ Object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md#object-plasma-engine-docum)| | |
| |[ OtherObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md#otherobject-plasma-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The number of contact points in this collision.
> ``` lang=cpp, name=Lightning
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactpointrange.md)

 `read-only`

> A range for iterating through all contact points.
> ``` lang=cpp, name=Lightning
> var ContactPoints : ContactPointRange


---  
 #  IsGhost : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> If this was a ghost collision (detected but not resolved).
> ``` lang=cpp, name=Lightning
> var IsGhost : Boolean


---  
 #  Object : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The object that this event was sent to.
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  OtherObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The other object in this collision.
> ``` lang=cpp, name=Lightning
> var OtherObject : Cog


---  
 #  Methods


---  
 

 
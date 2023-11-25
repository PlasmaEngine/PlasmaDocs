 `Physics`

(NOTE) A bi-directional graph edge between a collider and a contact. Exposes some internals to Contact which currently can't be exposed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#contactgraphedge-void)|[ ContactPointCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#contactpointcount-plasma-e)|BaseConstraintGraphEdge<Physics::Contact,Physics::ContactEdge>| |
| |[ ContactPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#contactpoints-plasma-engin)| | |
| |[ FirstPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#firstpoint-plasma-engine-d)| | |
| |[ IsGhost](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#isghost-plasma-engine-docu)| | |
| |[ Object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#object-plasma-engine-docum)| | |
| |[ OtherObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md#otherobject-plasma-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> How many points of contact were in this collision.
> ``` lang=cpp, name=Lightning
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactpointrange.md)

 `read-only`

> Returns a range of all contact points in the collision.
> ``` lang=cpp, name=Lightning
> var ContactPoints : ContactPointRange


---  
 #  FirstPoint : [contactpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactpoint.md)

 `read-only`

> Convenience function to return the first ContactPoint. Some logic only cares about one point of information. In a more general case all points should be iterated over.
> ``` lang=cpp, name=Lightning
> var FirstPoint : ContactPoint


---  
 #  IsGhost : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Was this a ghost collision?
> ``` lang=cpp, name=Lightning
> var IsGhost : Boolean


---  
 #  Object : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  OtherObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var OtherObject : Cog


---  
 #  Methods


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ContactGraphEdge()
> ``` 


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[contactgraphedge](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactgraphedge.md)| |
> ``` lang=cpp, name=Lightning
> function ContactGraphEdge( : ContactGraphEdge)
> ``` 


---  
 

 
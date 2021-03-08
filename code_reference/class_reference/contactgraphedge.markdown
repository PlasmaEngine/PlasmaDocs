 `Physics`

(NOTE) A bi-directional graph edge between a collider and a contact. Exposes some internals to Contact which currently can't be exposed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#contactgraphedge-void)|[ ContactPointCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#contactpointcount-plasma-e)|BaseConstraintGraphEdge<Physics::Contact,Physics::ContactEdge>| |
| |[ ContactPoints](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#contactpoints-plasma-engin)| | |
| |[ FirstPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#firstpoint-plasma-engine-d)| | |
| |[ IsGhost](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#isghost-plasma-engine-docu)| | |
| |[ Object](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#object-plasma-engine-docum)| | |
| |[ OtherObject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown#otherobject-plasma-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> How many points of contact were in this collision.
> ``` lang=cpp, name=Lightning
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactpointrange.markdown)

 `read-only`

> Returns a range of all contact points in the collision.
> ``` lang=cpp, name=Lightning
> var ContactPoints : ContactPointRange


---  
 #  FirstPoint : [contactpoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactpoint.markdown)

 `read-only`

> Convenience function to return the first ContactPoint. Some logic only cares about one point of information. In a more general case all points should be iterated over.
> ``` lang=cpp, name=Lightning
> var FirstPoint : ContactPoint


---  
 #  IsGhost : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Was this a ghost collision?
> ``` lang=cpp, name=Lightning
> var IsGhost : Boolean


---  
 #  Object : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  OtherObject : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

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
> ||[contactgraphedge](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/contactgraphedge.markdown)| |
> ``` lang=cpp, name=Lightning
> function ContactGraphEdge( : ContactGraphEdge)
> ``` 


---  
 

 
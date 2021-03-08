 `Physics`

(NOTE) A filter for storing the relationship between a pair of groups. Stores flags for the kind of filter this is, as well as what events to send out and to whom.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown#collisionfilter-void)|[ CollisionFlag](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown#collisionflag-plasma-engin)|[safeid32eventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/safeid32eventobject.markdown)| |
| |[ CollisionGroupA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown#collisiongroupa-plasma-eng)| | |
| |[ CollisionGroupB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown#collisiongroupb-plasma-eng)| | |


 #  Properties


---  
 #  CollisionFlag : [CollisionFilterCollisionFlags](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#collisionfiltercollisionflags)

> The collision state between the two types. Controls whether the types skip detection, skip resolution, or resolve as normal.
> ``` lang=cpp, name=Lightning
> var CollisionFlag : CollisionFilterCollisionFlags


---  
 #  CollisionGroupA : [collisiongroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CollisionGroupA : CollisionGroup


---  
 #  CollisionGroupB : [collisiongroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CollisionGroupB : CollisionGroup


---  
 #  Methods


---  
 #  CollisionFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CollisionFilter()
> ``` 


---  
 

 
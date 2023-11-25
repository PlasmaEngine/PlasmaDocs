 `Physics`

(NOTE) A filter for storing the relationship between a pair of groups. Stores flags for the kind of filter this is, as well as what events to send out and to whom.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilter.md#collisionfilter-void)|[ CollisionFlag](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilter.md#collisionflag-plasma-engin)|[safeid32eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32eventobject.md)| |
| |[ CollisionGroupA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilter.md#collisiongroupa-plasma-eng)| | |
| |[ CollisionGroupB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilter.md#collisiongroupb-plasma-eng)| | |


 #  Properties


---  
 #  CollisionFlag : [CollisionFilterCollisionFlags](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#collisionfiltercollisionflags)

> The collision state between the two types. Controls whether the types skip detection, skip resolution, or resolve as normal.
> ``` lang=cpp, name=Lightning
> var CollisionFlag : CollisionFilterCollisionFlags


---  
 #  CollisionGroupA : [collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CollisionGroupA : CollisionGroup


---  
 #  CollisionGroupB : [collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)

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
 

 
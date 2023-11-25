 `Resource` `Physics`



(NOTE) Defines filter pairs between CollisionGroups. These filters are used to control if collision detection and resolution happens between Colliders. Additionally, CollisionFilterBlocks can be defined on filters to send out extra events.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md#createruntime-plasma-engin)| |[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
|[ FindFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md#findfilter-plasma-engine-d)| | | |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md#runtimeclone-plasma-engine)| | | |


 #  Properties


---  
 #  Methods


---  
 #  CreateRuntime : [collisiontable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md)

 `static`

> Creates a CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : CollisionTable
> ``` 


---  
 #  FindFilter : [collisionfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilter.md)

> Finds the filter between the pair of collision groups.
> |Name|Type|Description|
> |---|---|---|
> |groupA|[collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)| |
> |groupB|[collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)| |
> ``` lang=cpp, name=Lightning
> function FindFilter(groupA : CollisionGroup, groupB : CollisionGroup) : CollisionFilter
> ``` 


---  
 #  RuntimeClone : [collisiontable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md)

> Creates a clone of this CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : CollisionTable
> ``` 


---  
 

 
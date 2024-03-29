 `Physics`

(NOTE) A helper class to create joints of various configurations. Each joint is configured from two points. Any other specific joint properties are calculated from these two points.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddJointLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#addjointlimit-plasma-engin)|[ AttachToCommonParent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#attachtocommonparent-zer)| | |
|[ AddJointMotor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#addjointmotor-plasma-engin)|[ AttachToWorld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#attachtoworld-plasma-engin)| | |
|[ AddJointSpring](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#addjointspring-plasma-engi)|[ AutoSnaps](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#autosnaps-plasma-engine-do)| | |
|[ Create](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#create-plasma-engine-docum)|[ OverrideLength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#overridelength-plasma-engi)| | |
|[ CreateLocalPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#createlocalpoints-plasma-e)|[ UseCenter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#usecenter-plasma-engine-do)| | |
|[ CreateWorldPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#createworldpoints-plasma-e)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointcreator.md#jointcreator-void)| | | |


 #  Properties


---  
 #  AttachToCommonParent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the cog of the joint be added as a child of the common parent of the two given cogs? Useful for putting the joint in the same hierarchy so that archetypes can be created.
> ``` lang=cpp, name=Lightning
> var AttachToCommonParent : Boolean


---  
 #  AttachToWorld : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Used to create a connection to a dummy object. Instead of connecting to object B, the connection will be between object A and "the world".
> ``` lang=cpp, name=Lightning
> var AttachToWorld : Boolean


---  
 #  AutoSnaps : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the joint auto-snap when the force limit is reached?
> ``` lang=cpp, name=Lightning
> var AutoSnaps : Boolean


---  
 #  OverrideLength : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the length of the joint be overridden or computed from the two points? Mainly used for StickJoint.
> ``` lang=cpp, name=Lightning
> var OverrideLength : Boolean


---  
 #  UseCenter : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the center of each object be used instead of the given points?
> ``` lang=cpp, name=Lightning
> var UseCenter : Boolean


---  
 #  Methods


---  
 #  AddJointLimit : [jointlimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md)

> Add a JointLimit to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AddJointLimit(joint : Cog) : JointLimit
> ``` 


---  
 #  AddJointMotor : [jointmotor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md)

> Add a JointMotor to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AddJointMotor(joint : Cog) : JointMotor
> ``` 


---  
 #  AddJointSpring : [jointspring](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointspring.md)

> Add a JointSpring to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AddJointSpring(joint : Cog) : JointSpring
> ``` 


---  
 #  Create : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function Create(objectA : Cog, objectB : Cog, jointArchetype : Archetype) : Cog
> ``` 


---  
 #  Create : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function Create(objectA : Cog, objectB : Cog, jointName : String) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> |localPointA|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |localPointB|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |localPointA|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |localPointB|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointName : String, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> |bothWorldPoints|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> |worldPointA|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |worldPointB|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |bothWorldPoints|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |worldPointA|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |worldPointB|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  JointCreator : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function JointCreator()
> ``` 


---  
 

 
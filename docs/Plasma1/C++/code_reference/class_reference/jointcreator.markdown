 `Physics`

(NOTE) A helper class to create joints of various configurations. Each joint is configured from two points. Any other specific joint properties are calculated from these two points.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddJointLimit](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#addjointlimit-plasma-engin)|[ AttachToCommonParent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#attachtocommonparent-zer)| | |
|[ AddJointMotor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#addjointmotor-plasma-engin)|[ AttachToWorld](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#attachtoworld-plasma-engin)| | |
|[ AddJointSpring](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#addjointspring-plasma-engi)|[ AutoSnaps](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#autosnaps-plasma-engine-do)| | |
|[ Create](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#create-plasma-engine-docum)|[ OverrideLength](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#overridelength-plasma-engi)| | |
|[ CreateLocalPoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#createlocalpoints-plasma-e)|[ UseCenter](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#usecenter-plasma-engine-do)| | |
|[ CreateWorldPoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#createworldpoints-plasma-e)| | | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointcreator.markdown#jointcreator-void)| | | |


 #  Properties


---  
 #  AttachToCommonParent : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Should the cog of the joint be added as a child of the common parent of the two given cogs? Useful for putting the joint in the same hierarchy so that archetypes can be created.
> ``` lang=cpp, name=Lightning
> var AttachToCommonParent : Boolean


---  
 #  AttachToWorld : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Used to create a connection to a dummy object. Instead of connecting to object B, the connection will be between object A and "the world".
> ``` lang=cpp, name=Lightning
> var AttachToWorld : Boolean


---  
 #  AutoSnaps : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Should the joint auto-snap when the force limit is reached?
> ``` lang=cpp, name=Lightning
> var AutoSnaps : Boolean


---  
 #  OverrideLength : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Should the length of the joint be overridden or computed from the two points? Mainly used for StickJoint.
> ``` lang=cpp, name=Lightning
> var OverrideLength : Boolean


---  
 #  UseCenter : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Should the center of each object be used instead of the given points?
> ``` lang=cpp, name=Lightning
> var UseCenter : Boolean


---  
 #  Methods


---  
 #  AddJointLimit : [jointlimit](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointlimit.markdown)

> Add a JointLimit to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddJointLimit(joint : Cog) : JointLimit
> ``` 


---  
 #  AddJointMotor : [jointmotor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointmotor.markdown)

> Add a JointMotor to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddJointMotor(joint : Cog) : JointMotor
> ``` 


---  
 #  AddJointSpring : [jointspring](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/jointspring.markdown)

> Add a JointSpring to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddJointSpring(joint : Cog) : JointSpring
> ``` 


---  
 #  Create : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointArchetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> ``` lang=cpp, name=Lightning
> function Create(objectA : Cog, objectB : Cog, jointArchetype : Archetype) : Cog
> ``` 


---  
 #  Create : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointName|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Create(objectA : Cog, objectB : Cog, jointName : String) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointArchetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> |localPointA|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |localPointB|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointName|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |localPointA|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |localPointB|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointName : String, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by archetype) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointArchetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> |bothWorldPoints|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointArchetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
> |worldPointA|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |worldPointB|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by component name) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointName|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |bothWorldPoints|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |objectB|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |jointName|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |worldPointA|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |worldPointB|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
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
 

 
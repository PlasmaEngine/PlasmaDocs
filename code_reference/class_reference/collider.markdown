 `Component` `Physics`



(NOTE) A collider controls how collision detection is performed for an object. A collider also gives mass properties to a RigidBody(via the material and volume). If there is no RigidBody associated with this collider then it is considered static. Note: colliders without RigidBodies should not be moved at run-time!

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeVolume](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#computevolume-plasma-engin)|[ ActiveBody](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#activebody-plasma-engine-d)|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)|[boxcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/boxcollider.markdown)|
|[ GetPointVelocity](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#getpointvelocity-plasma-en)|[ CollisionGroup](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#collisiongroup-plasma-engi)| |[capsulecollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/capsulecollider.markdown)|
| |[ ContactCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#contactcount-plasma-engine)| |[convexmeshcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/convexmeshcollider.markdown)|
| |[ Contacts](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#contacts-plasma-engine-doc)| |[cylindercollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cylindercollider.markdown)|
| |[ Ghost](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#ghost-plasma-engine-docume)| |[ellipsoidcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ellipsoidcollider.markdown)|
| |[ JointCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#jointcount-plasma-engine-d)| |[heightmapcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/heightmapcollider.markdown)|
| |[ Joints](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#joints-plasma-engine-docum)| |[meshcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/meshcollider.markdown)|
| |[ Material](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#material-plasma-engine-doc)| |[multiconvexmeshcollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/multiconvexmeshcollider.markdown)|
| |[ Offset](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#offset-plasma-engine-docum)| |[spherecollider](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/spherecollider.markdown)|
| |[ SendsEvents](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#sendsevents-plasma-engine)| | |
| |[ WorldAabb](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#worldaabb-plasma-engine-do)| | |
| |[ WorldBoundingSphere](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown#worldboundingsphere-plasma)| | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/rigidbody.markdown)

 `read-only`

> The rigid body that "owns" this collider. This is the body that forces/impulses/etc... should be applied to.
> ``` lang=cpp, name=Lightning
> var ActiveBody : RigidBody


---  
 #  CollisionGroup : [collisiongroup](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)

> The collision group is a tag used to alter collision behavior based upon the space's CollisionTable.
> ``` lang=cpp, name=Lightning
> var CollisionGroup : CollisionGroup


---  
 #  ContactCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> The current number of contacts/collisions with this collider.
> ``` lang=cpp, name=Lightning
> var ContactCount : Integer


---  
 #  Contacts : [contactrange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/contactrange.markdown)

 `read-only`

> A range of all contacts for this collider.
> ``` lang=cpp, name=Lightning
> var Contacts : ContactRange


---  
 #  Ghost : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Ghosted colliders do not resolve collision. They do still detect collisions and send events. Ghosted colliders are typically used for trigger regions.
> ``` lang=cpp, name=Lightning
> var Ghost : Boolean


---  
 #  JointCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> The number of joints attached to this collider.
> ``` lang=cpp, name=Lightning
> var JointCount : Integer


---  
 #  Joints : [jointrange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointrange.markdown)

 `read-only`

> A range of all joints attached to this collider.
> ``` lang=cpp, name=Lightning
> var Joints : JointRange


---  
 #  Material : [physicsmaterial](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicsmaterial.markdown)

> The material used to determine the density, restitution, and friction of this collider.
> ``` lang=cpp, name=Lightning
> var Material : PhysicsMaterial


---  
 #  Offset : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Moves the physics defined center of the object away from the transform's translation. Used to move physics to match a model.
> ``` lang=cpp, name=Lightning
> var Offset : Real3


---  
 #  SendsEvents : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Determines if this object will send collision events. Used mainly for increasing performance by not sending unnecessary collision events.
> ``` lang=cpp, name=Lightning
> var SendsEvents : Boolean


---  
 #  WorldAabb : [aabb](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)

 `read-only`

> Returns the world-space axis aligned bounding box (Aabb) of this collider.
> ``` lang=cpp, name=Lightning
> var WorldAabb : Aabb


---  
 #  WorldBoundingSphere : [sphere](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/sphere.markdown)

 `read-only`

> Returns the world-space bounding sphere of this collider.
> ``` lang=cpp, name=Lightning
> var WorldBoundingSphere : Sphere


---  
 #  Methods


---  
 #  ComputeVolume : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Compute the world-space volume of this collider.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ComputeVolume() : Real
> ``` 


---  
 #  GetPointVelocity : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Returns the point velocity of a world-space point with respect to the current rigid body's linear and angular velocity. If there is no rigid body this returns plasma.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 

 
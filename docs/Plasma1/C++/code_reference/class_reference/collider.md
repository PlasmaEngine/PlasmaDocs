 `Component` `Physics`



(NOTE) A collider controls how collision detection is performed for an object. A collider also gives mass properties to a RigidBody(via the material and volume). If there is no RigidBody associated with this collider then it is considered static. Note: colliders without RigidBodies should not be moved at run-time!

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#computevolume-plasma-engin)|[ ActiveBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#activebody-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)|[boxcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.md)|
|[ GetPointVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#getpointvelocity-plasma-en)|[ CollisionGroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#collisiongroup-plasma-engi)| |[capsulecollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.md)|
| |[ ContactCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#contactcount-plasma-engine)| |[convexmeshcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmeshcollider.md)|
| |[ Contacts](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#contacts-plasma-engine-doc)| |[cylindercollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cylindercollider.md)|
| |[ Ghost](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#ghost-plasma-engine-docume)| |[ellipsoidcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ellipsoidcollider.md)|
| |[ JointCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#jointcount-plasma-engine-d)| |[heightmapcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md)|
| |[ Joints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#joints-plasma-engine-docum)| |[meshcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md)|
| |[ Material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#material-plasma-engine-doc)| |[multiconvexmeshcollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshcollider.md)|
| |[ Offset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#offset-plasma-engine-docum)| |[spherecollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spherecollider.md)|
| |[ SendsEvents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#sendsevents-plasma-engine)| | |
| |[ WorldAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#worldaabb-plasma-engine-do)| | |
| |[ WorldBoundingSphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md#worldboundingsphere-plasma)| | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rigidbody.md)

 `read-only`

> The rigid body that "owns" this collider. This is the body that forces/impulses/etc... should be applied to.
> ``` lang=cpp, name=Lightning
> var ActiveBody : RigidBody


---  
 #  CollisionGroup : [collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)

> The collision group is a tag used to alter collision behavior based upon the space's CollisionTable.
> ``` lang=cpp, name=Lightning
> var CollisionGroup : CollisionGroup


---  
 #  ContactCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The current number of contacts/collisions with this collider.
> ``` lang=cpp, name=Lightning
> var ContactCount : Integer


---  
 #  Contacts : [contactrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactrange.md)

 `read-only`

> A range of all contacts for this collider.
> ``` lang=cpp, name=Lightning
> var Contacts : ContactRange


---  
 #  Ghost : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Ghosted colliders do not resolve collision. They do still detect collisions and send events. Ghosted colliders are typically used for trigger regions.
> ``` lang=cpp, name=Lightning
> var Ghost : Boolean


---  
 #  JointCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The number of joints attached to this collider.
> ``` lang=cpp, name=Lightning
> var JointCount : Integer


---  
 #  Joints : [jointrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointrange.md)

 `read-only`

> A range of all joints attached to this collider.
> ``` lang=cpp, name=Lightning
> var Joints : JointRange


---  
 #  Material : [physicsmaterial](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md)

> The material used to determine the density, restitution, and friction of this collider.
> ``` lang=cpp, name=Lightning
> var Material : PhysicsMaterial


---  
 #  Offset : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Moves the physics defined center of the object away from the transform's translation. Used to move physics to match a model.
> ``` lang=cpp, name=Lightning
> var Offset : Real3


---  
 #  SendsEvents : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this object will send collision events. Used mainly for increasing performance by not sending unnecessary collision events.
> ``` lang=cpp, name=Lightning
> var SendsEvents : Boolean


---  
 #  WorldAabb : [aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)

 `read-only`

> Returns the world-space axis aligned bounding box (Aabb) of this collider.
> ``` lang=cpp, name=Lightning
> var WorldAabb : Aabb


---  
 #  WorldBoundingSphere : [sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.md)

 `read-only`

> Returns the world-space bounding sphere of this collider.
> ``` lang=cpp, name=Lightning
> var WorldBoundingSphere : Sphere


---  
 #  Methods


---  
 #  ComputeVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Compute the world-space volume of this collider.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ComputeVolume() : Real
> ``` 


---  
 #  GetPointVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Returns the point velocity of a world-space point with respect to the current rigid body's linear and angular velocity. If there is no rigid body this returns plasma.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 

 
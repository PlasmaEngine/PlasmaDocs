 `Component` `Physics`



(NOTE) The PhysicsSpace is an "instance" of a world. This world manages and stores all of the other physical components of this world. PhysicSpaces act independently of each other.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddHierarchyPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#addhierarchypairfilter-v)|[ AllowSleep](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#allowsleep-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ AddPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#addpairfilter-void)|[ CollisionTable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#collisiontable-plasma-engi)| | |
|[ CastAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castaabb-plasma-engine-doc)|[ Deterministic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#deterministic-plasma-engin)| | |
|[ CastCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castcollider-plasma-engine)|[ DynamicBroadphaseType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#dynamicbroadphasetype-ze)| | |
|[ CastFrustum](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castfrustum-plasma-engine)|[ Mode2D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#mode2d-plasma-engine-docum)| | |
|[ CastRay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castray-plasma-engine-docu)|[ PhysicsSolverConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#physicssolverconfig-plasma)| | |
|[ CastRayFirst](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castrayfirst-plasma-engine)|[ StaticBroadphaseType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#staticbroadphasetype-zer)| | |
|[ CastSegment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castsegment-plasma-engine)|[ SubStepCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#substepcount-plasma-engine)| | |
|[ CastSphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#castsphere-plasma-engine-d)| | | |
|[ CreateJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#createjoint-plasma-engine)| | | |
|[ DispatchWithinAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#dispatchwithinaabb-void)| | | |
|[ DispatchWithinSphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#dispatchwithinsphere-voi)| | | |
|[ FlushPhysicsQueue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#flushphysicsqueue-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#physicsspace-void)| | | |
|[ RemoveHierarchyPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#removehierarchypairfilte)| | | |
|[ RemovePairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#removepairfilter-void)| | | |
|[ SweepCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#sweepcollider-plasma-engin)| | | |
|[ WhyAreTheyNotColliding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.md#whyaretheynotcolliding-z)| | | |


 #  Properties


---  
 #  AllowSleep : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if anything in the space is allowed to fall sleep.
> ``` lang=cpp, name=Lightning
> var AllowSleep : Boolean


---  
 #  CollisionTable : [collisiontable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.md)

> The collision table resource used to filter collisions in this space.
> ``` lang=cpp, name=Lightning
> var CollisionTable : CollisionTable


---  
 #  Deterministic : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Performs extra work to help enforce determinism in the simulation.
> ``` lang=cpp, name=Lightning
> var Deterministic : Boolean


---  
 #  DynamicBroadphaseType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> What kind of broadphase is used for dynamic objects (those with RigidBodies).
> ``` lang=cpp, name=Lightning
> var DynamicBroadphaseType : String


---  
 #  Mode2D : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> The default 2D mode for this space. If a RigidBody is set to InheritFromSpace then it will use this value.
> ``` lang=cpp, name=Lightning
> var Mode2D : Boolean


---  
 #  PhysicsSolverConfig : [physicssolverconfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md)

> The resource that controls how physics solves things. Mostly related to how collision is resolved.
> ``` lang=cpp, name=Lightning
> var PhysicsSolverConfig : PhysicsSolverConfig


---  
 #  StaticBroadphaseType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> What kind of broadphase is used for static objects (those without RigidBodies).
> ``` lang=cpp, name=Lightning
> var StaticBroadphaseType : String


---  
 #  SubStepCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of iterations the physics space will take every frame. Used to achieve higher accuracy and increase visual results.
> ``` lang=cpp, name=Lightning
> var SubStepCount : Integer


---  
 #  Methods


---  
 #  AddHierarchyPairFilter : Void

> Adds a filter to ignore collision between both hierarchies passed in. See AddPairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AddHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  AddPairFilter : Void

> Filters two cogs to not resolve collisions with each other. This is a runtime only feature and will not be saved.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AddPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  CastAabb : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that an Aabb hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastAabb(aabb : Aabb, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastCollider : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that another collider hits using the given filter. The test collider's position can be offset to test at a different location. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |offset|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |testCollider|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastCollider(offset : Real3, testCollider : Collider, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastFrustum : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a Frustum hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |frustum|[frustum](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frustum.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastFrustum(frustum : Frustum, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a ray hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function CastRay(worldRay : Ray, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a ray hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastRay(worldRay : Ray, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRayFirst : [castresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md)

> Finds the first collider that a ray hits. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> ``` lang=cpp, name=Lightning
> function CastRayFirst(worldRay : Ray) : CastResult
> ``` 


---  
 #  CastRayFirst : [castresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.md)

> Finds the first collider that a ray hits using the given filter.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastRayFirst(worldRay : Ray, filter : CastFilter) : CastResult
> ``` 


---  
 #  CastSegment : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a line segment hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function CastSegment(segment : Segment, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastSegment : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a line segment hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastSegment(segment : Segment, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastSphere : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.md)

> Finds all colliders in the space that a Sphere hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.md)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastSphere(sphere : Sphere, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CreateJoint : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Creates a joint by name (e.g. StickJoint) between two cogs. The world points of the joint are both set to worldPoint.
> |Name|Type|Description|
> |---|---|---|
> |cog0|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |worldPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function CreateJoint(cog0 : Cog, cog1 : Cog, jointName : String, worldPoint : Real3) : Cog
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinAabb(aabb : Aabb, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinAabb(aabb : Aabb, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinSphere(sphere : Sphere, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinSphere(sphere : Sphere, eventName : String, toSend : Event)
> ``` 


---  
 #  FlushPhysicsQueue : Void

> Forces all queued computations in physics to be updated now. Should only be used for debugging.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FlushPhysicsQueue()
> ``` 


---  
 #  PhysicsSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PhysicsSpace()
> ``` 


---  
 #  RemoveHierarchyPairFilter : Void

> Removes the filters between both hierarchies. See RemovePairFilter for more info.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  RemovePairFilter : Void

> Removes the filter between two cogs allowing collisions to be computed as normal.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function RemovePairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  SweepCollider : [sweepresultrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresultrange.md)

> Performs a swept cast with a collider's shape and a given velocity. Returns a range of all objects the collider could've hit within 'dt' time.
> |Name|Type|Description|
> |---|---|---|
> |collider|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
> |velocity|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |dt|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function SweepCollider(collider : Collider, velocity : Real3, dt : Real, filter : CastFilter) : SweepResultRange
> ``` 


---  
 #  WhyAreTheyNotColliding : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Returns a debug string stating why physics does or doesn't think these two objects should be colliding.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function WhyAreTheyNotColliding(cog1 : Cog, cog2 : Cog) : String
> ``` 


---  
 

 
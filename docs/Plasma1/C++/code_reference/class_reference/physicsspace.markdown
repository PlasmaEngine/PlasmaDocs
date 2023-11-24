 `Component` `Physics`



(NOTE) The PhysicsSpace is an "instance" of a world. This world manages and stores all of the other physical components of this world. PhysicSpaces act independently of each other.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddHierarchyPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#addhierarchypairfilter-v)|[ AllowSleep](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#allowsleep-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
|[ AddPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#addpairfilter-void)|[ CollisionTable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#collisiontable-plasma-engi)| | |
|[ CastAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castaabb-plasma-engine-doc)|[ Deterministic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#deterministic-plasma-engin)| | |
|[ CastCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castcollider-plasma-engine)|[ DynamicBroadphaseType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#dynamicbroadphasetype-ze)| | |
|[ CastFrustum](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castfrustum-plasma-engine)|[ Mode2D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#mode2d-plasma-engine-docum)| | |
|[ CastRay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castray-plasma-engine-docu)|[ PhysicsSolverConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#physicssolverconfig-plasma)| | |
|[ CastRayFirst](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castrayfirst-plasma-engine)|[ StaticBroadphaseType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#staticbroadphasetype-zer)| | |
|[ CastSegment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castsegment-plasma-engine)|[ SubStepCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#substepcount-plasma-engine)| | |
|[ CastSphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#castsphere-plasma-engine-d)| | | |
|[ CreateJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#createjoint-plasma-engine)| | | |
|[ DispatchWithinAabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#dispatchwithinaabb-void)| | | |
|[ DispatchWithinSphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#dispatchwithinsphere-voi)| | | |
|[ FlushPhysicsQueue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#flushphysicsqueue-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#physicsspace-void)| | | |
|[ RemoveHierarchyPairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#removehierarchypairfilte)| | | |
|[ RemovePairFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#removepairfilter-void)| | | |
|[ SweepCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#sweepcollider-plasma-engin)| | | |
|[ WhyAreTheyNotColliding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown#whyaretheynotcolliding-z)| | | |


 #  Properties


---  
 #  AllowSleep : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Determines if anything in the space is allowed to fall sleep.
> ``` lang=cpp, name=Lightning
> var AllowSleep : Boolean


---  
 #  CollisionTable : [collisiontable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiontable.markdown)

> The collision table resource used to filter collisions in this space.
> ``` lang=cpp, name=Lightning
> var CollisionTable : CollisionTable


---  
 #  Deterministic : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Performs extra work to help enforce determinism in the simulation.
> ``` lang=cpp, name=Lightning
> var Deterministic : Boolean


---  
 #  DynamicBroadphaseType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> What kind of broadphase is used for dynamic objects (those with RigidBodies).
> ``` lang=cpp, name=Lightning
> var DynamicBroadphaseType : String


---  
 #  Mode2D : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> The default 2D mode for this space. If a RigidBody is set to InheritFromSpace then it will use this value.
> ``` lang=cpp, name=Lightning
> var Mode2D : Boolean


---  
 #  PhysicsSolverConfig : [physicssolverconfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.markdown)

> The resource that controls how physics solves things. Mostly related to how collision is resolved.
> ``` lang=cpp, name=Lightning
> var PhysicsSolverConfig : PhysicsSolverConfig


---  
 #  StaticBroadphaseType : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> What kind of broadphase is used for static objects (those without RigidBodies).
> ``` lang=cpp, name=Lightning
> var StaticBroadphaseType : String


---  
 #  SubStepCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

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
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  AddPairFilter : Void

> Filters two cogs to not resolve collisions with each other. This is a runtime only feature and will not be saved.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  CastAabb : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that an Aabb hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastAabb(aabb : Aabb, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastCollider : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that another collider hits using the given filter. The test collider's position can be offset to test at a different location. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |offset|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |testCollider|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastCollider(offset : Real3, testCollider : Collider, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastFrustum : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a Frustum hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |frustum|[frustum](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frustum.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastFrustum(frustum : Frustum, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a ray hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastRay(worldRay : Ray, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastRay : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a ray hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastRay(worldRay : Ray, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastRayFirst : [castresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.markdown)

> Finds the first collider that a ray hits. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastRayFirst(worldRay : Ray) : CastResult
> ``` 


---  
 #  CastRayFirst : [castresult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresult.markdown)

> Finds the first collider that a ray hits using the given filter.
> |Name|Type|Description|
> |---|---|---|
> |worldRay|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastRayFirst(worldRay : Ray, filter : CastFilter) : CastResult
> ``` 


---  
 #  CastSegment : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a line segment hits. This returns up to maxCount number of objects. A default CastFilter will be used.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastSegment(segment : Segment, maxCount : Integer) : CastResultsRange
> ``` 


---  
 #  CastSegment : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a line segment hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastSegment(segment : Segment, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CastSphere : [castresultsrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castresultsrange.markdown)

> Finds all colliders in the space that a Sphere hits using the given filter. This returns up to maxCount number of objects.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.markdown)| |
> |maxCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastSphere(sphere : Sphere, maxCount : Integer, filter : CastFilter) : CastResultsRange
> ``` 


---  
 #  CreateJoint : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> Creates a joint by name (e.g. StickJoint) between two cogs. The world points of the joint are both set to worldPoint.
> |Name|Type|Description|
> |---|---|---|
> |cog0|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |jointName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |worldPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateJoint(cog0 : Cog, cog1 : Cog, jointName : String, worldPoint : Real3) : Cog
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinAabb(aabb : Aabb, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinAabb : Void

> Dispatches an event to all objects within the given aabb. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.markdown)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinAabb(aabb : Aabb, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere using the provided cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchWithinSphere(sphere : Sphere, filter : CastFilter, eventName : String, toSend : Event)
> ``` 


---  
 #  DispatchWithinSphere : Void

> Dispatches an event to all objects within the given sphere. Uses the default cast filter.
> |Name|Type|Description|
> |---|---|---|
> |sphere|[sphere](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphere.markdown)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
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
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveHierarchyPairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  RemovePairFilter : Void

> Removes the filter between two cogs allowing collisions to be computed as normal.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemovePairFilter(cog1 : Cog, cog2 : Cog)
> ``` 


---  
 #  SweepCollider : [sweepresultrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sweepresultrange.markdown)

> Performs a swept cast with a collider's shape and a given velocity. Returns a range of all objects the collider could've hit within 'dt' time.
> |Name|Type|Description|
> |---|---|---|
> |collider|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)| |
> |velocity|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |dt|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |filter|[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function SweepCollider(collider : Collider, velocity : Real3, dt : Real, filter : CastFilter) : SweepResultRange
> ``` 


---  
 #  WhyAreTheyNotColliding : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> Returns a debug string stating why physics does or doesn't think these two objects should be colliding.
> |Name|Type|Description|
> |---|---|---|
> |cog1|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |cog2|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function WhyAreTheyNotColliding(cog1 : Cog, cog2 : Cog) : String
> ``` 


---  
 

 
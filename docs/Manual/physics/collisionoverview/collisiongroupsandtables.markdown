[ CollisionGroups](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown) and [ CollisionTables](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiontable.markdown) are intertwined resources in the physics system. A CollisionGroup defines a label for a [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/colliders.markdown) to be used within a CollisionTable. A CollisionTable defines filters for pairs of CollisionGroups. These filters allow extra control over what collisions can take place. Additionally, filters can be configured to send extra events.

 #  CollisionGroup
A CollisionGroup defines a group (or label) for a Collider to take part in. This only serves to group certain Colliders together but doesn't change any behavior unless the active CollisionTable is configured to do so.

 #  CollisionTable
A CollisionTable is a resource property set on [PhysicsSpace](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/physicsspace.markdown) that defines pair-wise CollisionGroup relationships known as CollisionFilters. These filters control if a collision happens and if extra events are sent between group pairings.

 ##  CollisionFilters
A [CollisionFilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown) can be used to control if collisions happen between pairs of CollisionGroups. There are three primary states of a CollisionFilter:
 - **Resolve:** The default state for a filter. Says that collision resolution should happen as normal.
 - **SkipResolution:** Collision detection should be run as normal but resolution should not happen. This allows configuring pairs to be ghost collisions while still getting events.
 - **SkipDetection:** Collision detection should be skipped. Skipping collision detection also implies skipping collision resolution. This option is typically only set for performance reasons. This can also be used to prevent collision events from being sent to make gameplay logic easier.
 
Additional information can be configured on a [CollisionFilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown) to send out events through the use of CollisionFilterBlocks.

 ###  CollisionFilterBlocks
A [CollisionFilterBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown) is a sub-component on CollisionFilter used to control what kinds of events are sent out between groups. The current supported block types are:
 - **CollisionStartBlock:** Sends out the GroupCollisionStarted event when this grouping has a CollisionStarted.
 - **CollisionPersistedBlock:** Sends out the GroupCollisionPersisted event when this grouping has a CollisionPersisted.
 - **CollisionEndBlock:** Sends out the GroupCollisionEnded event when this grouping has a CollisionEnded.
 - **PreSolveBlock:** Sent out before collision is resolved. Allows altering information before a collision has happened.
 
All blocks can configure which groups in the filter to send to. The `SendEventsTo` properties control which objects in the pairing should get the event. The `A` and `B` referred to are in the same order as the GroupA  and GroupB  properties of the filter. If a filter has GroupA and GroupB as the same value, then this order is not defined.

Additionally, filter blocks contain the EventOverride  property that lets the user send out a custom event name instead of the default names. Note that these names do not currently show up in the `Events` namespace and must be connected to with a string literal.

The PreSolveBlock is a special block that should be used sparingly. As [PreSolveEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/presolveevent.markdown) before collisions are resolved. This event does not expect any drastic changes to the scene, such as removing components. Any complex behavior other than changing property values may crash the engine.

 #  Troubleshooting
One of the most common issues when using CollisionGroups and CollisionTables is forgetting to set the correct CollisionTable resource on the [PhysicsSpace](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/physicsspace.markdown). Additionally, see [WhyAreTheyNotColliding](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/physicstroubleshooting/whyaretheynotcolliding.markdown) for other common collision issues.

---
 #  Related Materials
 ##  Manual
- [collisionevents.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/collisionevents.markdown)
- [physicsspace.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/physicsspace.markdown)
- [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/colliders.markdown)
- [whyaretheynotcolliding.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/physics/collisionoverview/physicstroubleshooting/whyaretheynotcolliding.markdown)

 ##  Reference
- [CollisionGroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)
- [CollisionTable](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiontable.markdown)
- [CollisionFilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilter.markdown)
- [CollisionEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionevent.markdown)
- [CollisionGroupEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroupevent.markdown)
- [PreSolveEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/presolveevent.markdown)
- [CollisionFilterBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown)
- [CollisionStartBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionstartblock.markdown)
- [CollisionPersistedBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionpersistedblock.markdown)
- [CollisionEndBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionendblock.markdown)
- [PreSolveBlock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/presolveblock.markdown) 

 
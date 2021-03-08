The [Collider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown) component is used to define a shape for collision detection. Together with the [RigidBody](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/rigidbody.markdown) component, this creates a game object for physics to move around. There are several pre-defined Collider types, as well as a few customizable types to choose from.
 - [BoxCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/boxcollider.markdown)
 - [SphereCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/spherecollider.markdown)
 - [CylinderCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/cylindercollider.markdown)
 - [EllipsoidCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/ellipsoidcollider.markdown)
 - [CapsuleCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/capsulecollider.markdown)
 - [MeshCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/meshcollider.markdown)
 - [ConvexMeshCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/convexmeshcollider.markdown)
 - [MultiConvexMeshCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/multiconvexmeshcollider.markdown)
 - [HeightMapCollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/colliders/heightmapcollider.markdown)

 #  The Collider Interface
A Collider is an interface component. This means only derived Collider types can be added to an object, not the base type. The Collider interface allows accessing common properties, such as ghost, between all Colliders without knowing the specific derived type.

 #  Colliders and RigidBodies
Colliders are used in combination with a [RigidBody](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/rigidbody.markdown) to give an object mass. The simplest object is one that has both a Collider and a RigidBody. See [Hierarchies](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/hierarchies.markdown) for more details. In either case, a Collider exposes the `ActiveBody` property to know what RigidBody a collider should apply forces to.

 #  Physics Material
The [PhysicsMaterial](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicsmaterial.markdown) on a Collider is used to determine how collision resolution should be handled. Knowing: 

(NOTE) mass = volume * density

the density on the material is used with the Collider's volume (implicit from the shape and size) to contribute mass and inertia to a RigidBody. Additionally the material defines surface properties such as friction and restitution which describe how energy is lost in a collision.

 #  Ghost Colliders
While a collider is often used to define a shape for collision resolution, it is also common to disable collision resolution through the {nav icon=check-square-o, name="Ghost"} property. The ghost property only disables collision resolution while continuing to detect collision. This is useful to create trigger regions where a user can check if something enters or exits an area. Additionally, ghost Colliders are often used to apply forces in an area with the Region component and [PhysicsEffects](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicseffectsandregions.markdown).

 #  Collision Groups
Sometimes a Collider should only collide with some objects. In this case the ghost property is not sufficient. One of the provided alternatives is to use the {nav icon=wrench, name="CollisionGroup"} property, which defines a group to be used in a CollisionTable. This allows customizing what group pairs go through collision detection and resolution. See [Collision Groups and Collision Tables](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/collisionoverview/collisiongroupsandtables.markdown) for more details.

 #  Collision Information
A Collider has two main methods of providing contact information (i.e. what other Colliders are in contact with this one). The most common way to do this is through [Collision Events](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/collisionoverview/collisionevents.markdown), which are sent to both objects involved in the contact by default. Additionally, a Collider exposes a range of current contacts to iterate through. In the same way, [Joints](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/joints.markdown) can also be iterated through.

---

 ##  Related Materials
 ###  Manual
 - [rigidbody.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/rigidbody.markdown)
 - [physicsmaterial.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicsmaterial.markdown)
 - [collisiongroupsandtables.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/collisionoverview/collisiongroupsandtables.markdown)
 - [collisionevents.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/collisionoverview/collisionevents.markdown)
 - [physicseffectsandregions.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicseffectsandregions.markdown)
 - [hierarchies.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/hierarchies.markdown)
 - [joints.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/joints.markdown)

 ###  Reference
 - [Collider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown)
 - [RigidBody](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rigidbody.markdown)
 - [PhysicsEffect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicseffect.markdown)
 - [Region](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/region.markdown)
 - [CollisionEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionevent.markdown)
 - [CollisionTable](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiontable.markdown)
 - [CollisionGroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)
 - [PhysicsMaterial](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicsmaterial.markdown)
 - [Joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)
 

 
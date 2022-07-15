# Thrust Effect
The [ThrustEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/thrusteffect.markdown) component applies a directional force at the center of the attached object. Note that this is different than applying the force through the object's center of mass. If the attached object's center differs from the center of mass then this will apply both a linear and angular force. This effect is often used for thrusters on a ship or other point forces that need to apply torque.

# Application Methods
The ThrustEffect component expects to be used as a [Collider](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/colliders.markdown) or Hierarchy effect. These application methods allow the thrust's center to be defined independently of the center of mass of the [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/rigidbody.markdown) If used as a RigidBody effect then this is no different than [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/forceeffect.markdown). Other application modes are undefined.

# Related Materials
## Manual
- [physicseffectsandregions.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions.markdown)
- [forceeffect.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/forceeffect.markdown)
- [rigidbody.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/rigidbody.markdown)
- [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/colliders.markdown)

## Reference
- [ThrustEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/thrusteffect.markdown)
- [PhysicsEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/physicseffect.markdown) 

 
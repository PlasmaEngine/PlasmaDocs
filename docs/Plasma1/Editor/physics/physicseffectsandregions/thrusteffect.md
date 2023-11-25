# Thrust Effect
The [ThrustEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.md) component applies a directional force at the center of the attached object. Note that this is different than applying the force through the object's center of mass. If the attached object's center differs from the center of mass then this will apply both a linear and angular force. This effect is often used for thrusters on a ship or other point forces that need to apply torque.

# Application Methods
The ThrustEffect component expects to be used as a [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/colliders.md) or Hierarchy effect. These application methods allow the thrust's center to be defined independently of the center of mass of the [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/rigidbody.md) If used as a RigidBody effect then this is no different than [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/forceeffect.md). Other application modes are undefined.

# Related Materials
## Manual
- [physicseffectsandregions.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions.md)
- [forceeffect.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/forceeffect.md)
- [rigidbody.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/rigidbody.md)
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/colliders.md)

## Reference
- [ThrustEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.md)
- [PhysicsEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md) 

 
# Force Effect
The [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/forceeffect.md) and [GravityEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gravityeffect.md) components are direction effects that apply linear forces to push an object in a direction.

The only difference between the gravity and force effect is whether an acceleration or force is applied. A GravityEffect will apply a constant acceleration to an object, i.e. the object's mass will not affect the acceleration. ForceEffect will take the object's mass into account. The rest of this page will use *force* to refer to the acceleration or force depending on the effect type attached.

The *force// applied is a constant linear //force* based upon the direction and strength of the effect. By default, the effect will be applied in the local space of the object it's attached to. This means that rotating the object will affect the direction of the //force//.

# Application Methods
GravityEffect and ForceEffect are assumed to work with all application methods of PhysicsEffects. If the effect is on the Space or LevelSettings then the *force* will apply to all objects in the level. If the effect is on a Region then it'll apply to all objects in the region. Otherwise, the effect will apply to the center of mass of the [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/rigidbody.md) (no angular //force//). [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/colliders.md) and Hierarchy application methods do not differ from the RigidBody mode.

# Related Materials
## Manual
- [physicseffectsandregions.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions.md)
- [rigidbody.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/rigidbody.md)
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/colliders.md)

## Reference
- [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/forceeffect.md)
- [GravityEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gravityeffect.md)
- [PhysicsEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)
- [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rigidbody.md)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md) 

 
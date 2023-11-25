# Linear Particle Animator
The linear particle animator give particles the ability to move.  It adds an integration step which allows particles to have some physically based motion.  The [LinearParticleAnimator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearparticleanimator.md) component is required to generate particles and and to move them.

(NOTE)**Where to set particle velocity?** Properties relating to velocity are not found on the `LinearParticleAnimator`, but are instead on the emitter component.  The reason for this property placement is that all properties on the [emitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/particles/emitters.md) component are applied when a particle is created, whereas the properties from `LinearParticleAnimator` are applied every frame.

# Forces
Both Force  and RandomForce  are used to apply forces to a particle.  The force will effect the velocity, which in turn effects the position of each particle.  If the RandomForce  defines the half-vector for a bounding box, then the random component of this frames Force is confined to this box.

# Growth
The Growth  property can change the size of particles over time.  Set Growth  to a positive number to make it grow, and a negative number to make it shrink.

![ParticleSystems_Growth](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46666.gif)

# Related Material
## Manual
- [Physics Effects and Regions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions.md)

## Code Reference
- [SpriteParticleSystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/spriteparticlesystem.md)
- [LinearParticleAnimator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearparticleanimator.md) 

 
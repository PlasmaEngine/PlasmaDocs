# Emitters
Emitters are necessary components for a particle system that define the properties of a particle as it's created.  One of those properties is the spawn position, which is in part defined by the component itself.  The emitter types are [BoxParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxparticleemitter.md), [SphericalParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphericalparticleemitter.md), and [MeshParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshparticleemitter.md), and each one defines a surface or curve that particles emit from.

NOTE: By default the shape isn't apparent on the Box or Sphere particle emitter.  This is because the EmitterSize  is zeroed out by default.

# Variance
Some properties on an emitter have a variance property to match.  Each particle inherits its properties from the emitter by adding a random value from variance to base value.  For example, two common properties for emitters are Size  and SizeVariance .  If Size  were set to `1` and the SizeVariance  was `0.1`, the size of each particle would be a random value in the range `[0.9,1.1]`.  The property StartVelocity  also has the variance counterpart RandomVelocity .  The velocity vector is computed similarly with a variance property, where the X, Y, and Z components of the vector are computed independently.

# Fast Emitters
When an object is moving fast, the fact that its motion is an illusion becomes more apparent.  When the gaps between the small teleportations grow bigger, the illusion is lost.  The illusion of motion is even harder to keep when a particle system is moving since the particles tend to trace the path of the object.  One way to fix this is to use a high EmitRate  and turn on FastMovingEmitter checkBox.  This will emit some of the extra particles between the gaps of the current and previous positions.

![ParticleSystems_FastMovingEmitter](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46688.gif) *Two particle emitters in motion, where the right one is using FastMovingEmitter checkBox*

# Related Material
## Manual
- [Color Gradient](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/architecture/resources/colorgradient.md)

## Code Reference
- [SpriteParticleSystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/spriteparticlesystem.md)
- [BoxParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxparticleemitter.md)
- [SphericalParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphericalparticleemitter.md)
- [MeshParticleEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshparticleemitter.md)
 

 
 `Component` `Graphics`



(NOTE) A particle system that uses sprites to represent each particle.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#spriteparticlesystem-voi)|[ BeamBaseScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#beambasescale-plasma-engin)|[particlesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md)| |
| |[ BeamVelocityScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#beamvelocityscale-plasma-e)| | |
| |[ GeometryMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#geometrymode-plasma-engine)| | |
| |[ ParticleAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#particleanimation-plasma-e)| | |
| |[ ParticleSort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#particlesort-plasma-engine)| | |
| |[ SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#spritesource-plasma-engine)| | |
| |[ VertexColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md#vertexcolor-plasma-engine)| | |


 #  Properties


---  
 #  BeamBaseScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much to scale particles along their direction of movement.
> ``` lang=cpp, name=Lightning
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much additional scale to add to particles by how fast they are moving.
> ``` lang=cpp, name=Lightning
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ``` lang=cpp, name=Lightning
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ``` lang=cpp, name=Lightning
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ``` lang=cpp, name=Lightning
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritesource.md)

> The sprite definition to use for each particle.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Color attribute of the generated vertices accessible in the vertex shader, value is multiplied with the particle color.
> ``` lang=cpp, name=Lightning
> var VertexColor : Real4


---  
 #  Methods


---  
 #  SpriteParticleSystem : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SpriteParticleSystem()
> ``` 


---  
 

 
 `Component` `Graphics`



(NOTE) A particle system that uses sprites to represent each particle.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#spriteparticlesystem-voi)|[ BeamBaseScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#beambasescale-plasma-engin)|[particlesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.markdown)| |
| |[ BeamVelocityScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#beamvelocityscale-plasma-e)| | |
| |[ GeometryMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#geometrymode-plasma-engine)| | |
| |[ ParticleAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#particleanimation-plasma-e)| | |
| |[ ParticleSort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#particlesort-plasma-engine)| | |
| |[ SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#spritesource-plasma-engine)| | |
| |[ VertexColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.markdown#vertexcolor-plasma-engine)| | |


 #  Properties


---  
 #  BeamBaseScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much to scale particles along their direction of movement.
> ``` lang=cpp, name=Lightning
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much additional scale to add to particles by how fast they are moving.
> ``` lang=cpp, name=Lightning
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ``` lang=cpp, name=Lightning
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ``` lang=cpp, name=Lightning
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ``` lang=cpp, name=Lightning
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritesource.markdown)

> The sprite definition to use for each particle.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.markdown)

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
 

 
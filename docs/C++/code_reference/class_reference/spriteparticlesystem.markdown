 `Component` `Graphics`



(NOTE) A particle system that uses sprites to represent each particle.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#spriteparticlesystem-voi)|[ BeamBaseScale](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#beambasescale-plasma-engin)|[particlesystem](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/particlesystem.markdown)| |
| |[ BeamVelocityScale](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#beamvelocityscale-plasma-e)| | |
| |[ GeometryMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#geometrymode-plasma-engine)| | |
| |[ ParticleAnimation](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#particleanimation-plasma-e)| | |
| |[ ParticleSort](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#particlesort-plasma-engine)| | |
| |[ SpriteSource](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#spritesource-plasma-engine)| | |
| |[ VertexColor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spriteparticlesystem.markdown#vertexcolor-plasma-engine)| | |


 #  Properties


---  
 #  BeamBaseScale : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> How much to scale particles along their direction of movement.
> ``` lang=cpp, name=Lightning
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> How much additional scale to add to particles by how fast they are moving.
> ``` lang=cpp, name=Lightning
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ``` lang=cpp, name=Lightning
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ``` lang=cpp, name=Lightning
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ``` lang=cpp, name=Lightning
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritesource.markdown)

> The sprite definition to use for each particle.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

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
 

 
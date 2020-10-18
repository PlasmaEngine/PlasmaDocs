 `Component` `Graphics`



(NOTE) An interface for generating and managing particles of a generic definition using emitters and animators.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AllParticles](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#allparticles-plasma-engine)|[ BoundingBoxSize](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#boundingboxsize-plasma-eng)|[graphical](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/graphical.markdown)|[spriteparticlesystem](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/spriteparticlesystem.markdown)|
|[ Clear](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#clear-void)|[ ChildSystem](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#childsystem-plasma-engine)| | |
| |[ PreviewInEditor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#previewineditor-plasma-eng)| | |
| |[ SystemSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#systemspace-plasma-engine)| | |
| |[ WarmUpTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlesystem.markdown#warmuptime-plasma-engine-d)| | |


 #  Properties


---  
 #  BoundingBoxSize : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Size of all sides of the bounding box used for frustum culling.
> ``` lang=cpp, name=Lightning
> var BoundingBoxSize : Real


---  
 #  ChildSystem : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If set, particle emission will happen for each particle in a parent system.
> ``` lang=cpp, name=Lightning
> var ChildSystem : Boolean


---  
 #  PreviewInEditor : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If the particle system should run on frame update in the editor instead of logic update.
> ``` lang=cpp, name=Lightning
> var PreviewInEditor : Boolean


---  
 #  SystemSpace : [SystemSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#systemspace)

> If particles are emitted into world space or if transform data remains relative to the transform of the system object.
> ``` lang=cpp, name=Lightning
> var SystemSpace : SystemSpace


---  
 #  WarmUpTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The amount of time to simulate the particle system on startup. This will be done on AllObjectsCreated, and will use the engines dt. This is good for when you want the particle effect to be in full bloom when you first see it. However, it can hurt performance at high values on startup.
> ``` lang=cpp, name=Lightning
> var WarmUpTime : Real


---  
 #  Methods


---  
 #  AllParticles : [particlelistrange](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/particlelistrange.markdown)

> A list of all particles currently active in the system.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AllParticles() : ParticleListRange
> ``` 


---  
 #  Clear : Void

> Clear all current particles.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 

 
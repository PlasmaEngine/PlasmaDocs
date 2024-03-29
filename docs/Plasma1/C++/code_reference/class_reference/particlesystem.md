 `Component` `Graphics`



(NOTE) An interface for generating and managing particles of a generic definition using emitters and animators.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AllParticles](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#allparticles-plasma-engine)|[ BoundingBoxSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#boundingboxsize-plasma-eng)|[graphical](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/graphical.md)|[spriteparticlesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spriteparticlesystem.md)|
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#clear-void)|[ ChildSystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#childsystem-plasma-engine)| | |
| |[ PreviewInEditor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#previewineditor-plasma-eng)| | |
| |[ SystemSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#systemspace-plasma-engine)| | |
| |[ WarmUpTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlesystem.md#warmuptime-plasma-engine-d)| | |


 #  Properties


---  
 #  BoundingBoxSize : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Size of all sides of the bounding box used for frustum culling.
> ``` lang=cpp, name=Lightning
> var BoundingBoxSize : Real


---  
 #  ChildSystem : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If set, particle emission will happen for each particle in a parent system.
> ``` lang=cpp, name=Lightning
> var ChildSystem : Boolean


---  
 #  PreviewInEditor : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If the particle system should run on frame update in the editor instead of logic update.
> ``` lang=cpp, name=Lightning
> var PreviewInEditor : Boolean


---  
 #  SystemSpace : [SystemSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#systemspace)

> If particles are emitted into world space or if transform data remains relative to the transform of the system object.
> ``` lang=cpp, name=Lightning
> var SystemSpace : SystemSpace


---  
 #  WarmUpTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The amount of time to simulate the particle system on startup. This will be done on AllObjectsCreated, and will use the engines dt. This is good for when you want the particle effect to be in full bloom when you first see it. However, it can hurt performance at high values on startup.
> ``` lang=cpp, name=Lightning
> var WarmUpTime : Real


---  
 #  Methods


---  
 #  AllParticles : [particlelistrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particlelistrange.md)

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
 

 
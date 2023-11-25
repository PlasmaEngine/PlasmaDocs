 `Component` `Graphics`



(NOTE) Particle Emitter Shared.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#resetcount-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#active-plasma-engine-docum)|[particleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemitter.md)|[boxparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxparticleemitter.md)|
| |[ EmitCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emitcount-plasma-engine-do)| |[meshparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshparticleemitter.md)|
| |[ EmitDelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emitdelay-plasma-engine-do)| |[sphericalparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphericalparticleemitter.md)|
| |[ EmitRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emitrate-plasma-engine-doc)| |[splineparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleemitter.md)|
| |[ EmitRateSoftStartTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emitratesoftstarttime-ze)| | |
| |[ EmitterSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emittersize-plasma-engine)| | |
| |[ EmitterVelocityPercent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emittervelocitypercent-z)| | |
| |[ EmitVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#emitvariance-plasma-engine)| | |
| |[ FastMovingEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#fastmovingemitter-plasma-e)| | |
| |[ Fill](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#fill-plasma-engine-documen)| | |
| |[ Lifetime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#lifetime-plasma-engine-doc)| | |
| |[ LifetimeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#lifetimevariance-plasma-en)| | |
| |[ RandomSpin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#randomspin-plasma-engine-d)| | |
| |[ RandomVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#randomvelocity-plasma-engi)| | |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#size-plasma-engine-documen)| | |
| |[ SizeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#sizevariance-plasma-engine)| | |
| |[ Spin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#spin-plasma-engine-documen)| | |
| |[ SpinVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#spinvariance-plasma-engine)| | |
| |[ StartVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#startvelocity-plasma-engin)| | |
| |[ TangentVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.md#tangentvelocity-plasma-eng)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is this emitter currently emitting particles?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  EmitCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Number of particles to emit per reset.
> ``` lang=cpp, name=Lightning
> var EmitCount : Integer


---  
 #  EmitDelay : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Time in seconds to delay the emission of particles from time of creation.
> ``` lang=cpp, name=Lightning
> var EmitDelay : Real


---  
 #  EmitRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Rate that particles spawn per second.
> ``` lang=cpp, name=Lightning
> var EmitRate : Real


---  
 #  EmitRateSoftStartTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Slowly ramps up to EmitRate over this time.
> ``` lang=cpp, name=Lightning
> var EmitRateSoftStartTime : Real


---  
 #  EmitterSize : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Size of the emitter.
> ``` lang=cpp, name=Lightning
> var EmitterSize : Real3


---  
 #  EmitterVelocityPercent : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much of the objects velocity is added to the particles.
> ``` lang=cpp, name=Lightning
> var EmitterVelocityPercent : Real


---  
 #  EmitVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the emit can vary per sample.
> ``` lang=cpp, name=Lightning
> var EmitVariance : Real


---  
 #  FastMovingEmitter : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not we attempt to emit along the vector between the previous position to the current position, which looks better for fast moving particle systems Note: Particle systems that teleport will emit along the teleport line.
> ``` lang=cpp, name=Lightning
> var FastMovingEmitter : Boolean


---  
 #  Fill : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much area of the emitter to used 0 to 1.
> ``` lang=cpp, name=Lightning
> var Fill : Real


---  
 #  Lifetime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How a particle's starting lifetime is.
> ``` lang=cpp, name=Lightning
> var Lifetime : Real


---  
 #  LifetimeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much lifetime can vary per particle.
> ``` lang=cpp, name=Lightning
> var LifetimeVariance : Real


---  
 #  RandomSpin : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Each particle should start with random spin.
> ``` lang=cpp, name=Lightning
> var RandomSpin : Boolean


---  
 #  RandomVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Random Velocity per particle.
> ``` lang=cpp, name=Lightning
> var RandomVelocity : Real3


---  
 #  Size : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Size of each particle spawned.
> ``` lang=cpp, name=Lightning
> var Size : Real


---  
 #  SizeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much the size can vary from the base size per particle.
> ``` lang=cpp, name=Lightning
> var SizeVariance : Real


---  
 #  Spin : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Speed in rads per second of the particle.
> ``` lang=cpp, name=Lightning
> var Spin : Real


---  
 #  SpinVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much spin speed can vary per particle.
> ``` lang=cpp, name=Lightning
> var SpinVariance : Real


---  
 #  StartVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Velocity of each particle at start.
> ``` lang=cpp, name=Lightning
> var StartVelocity : Real3


---  
 #  TangentVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Velocity of each particle in x horizontal tangent y vertical tangent and z outward tangent.
> ``` lang=cpp, name=Lightning
> var TangentVelocity : Real3


---  
 #  Methods


---  
 #  ResetCount : Void

> Reset the number of particles to emit back to EmitCount.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ResetCount()
> ``` 


---  
 

 
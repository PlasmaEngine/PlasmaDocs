 `Component` `Graphics`



(NOTE) Particle Emitter Shared.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#resetcount-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#active-plasma-engine-docum)|[particleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemitter.markdown)|[boxparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxparticleemitter.markdown)|
| |[ EmitCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emitcount-plasma-engine-do)| |[meshparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshparticleemitter.markdown)|
| |[ EmitDelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emitdelay-plasma-engine-do)| |[sphericalparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sphericalparticleemitter.markdown)|
| |[ EmitRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emitrate-plasma-engine-doc)| |[splineparticleemitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splineparticleemitter.markdown)|
| |[ EmitRateSoftStartTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emitratesoftstarttime-ze)| | |
| |[ EmitterSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emittersize-plasma-engine)| | |
| |[ EmitterVelocityPercent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emittervelocitypercent-z)| | |
| |[ EmitVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#emitvariance-plasma-engine)| | |
| |[ FastMovingEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#fastmovingemitter-plasma-e)| | |
| |[ Fill](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#fill-plasma-engine-documen)| | |
| |[ Lifetime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#lifetime-plasma-engine-doc)| | |
| |[ LifetimeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#lifetimevariance-plasma-en)| | |
| |[ RandomSpin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#randomspin-plasma-engine-d)| | |
| |[ RandomVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#randomvelocity-plasma-engi)| | |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#size-plasma-engine-documen)| | |
| |[ SizeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#sizevariance-plasma-engine)| | |
| |[ Spin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#spin-plasma-engine-documen)| | |
| |[ SpinVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#spinvariance-plasma-engine)| | |
| |[ StartVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#startvelocity-plasma-engin)| | |
| |[ TangentVelocity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/particleemittershared.markdown#tangentvelocity-plasma-eng)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Is this emitter currently emitting particles?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  EmitCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Number of particles to emit per reset.
> ``` lang=cpp, name=Lightning
> var EmitCount : Integer


---  
 #  EmitDelay : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Time in seconds to delay the emission of particles from time of creation.
> ``` lang=cpp, name=Lightning
> var EmitDelay : Real


---  
 #  EmitRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Rate that particles spawn per second.
> ``` lang=cpp, name=Lightning
> var EmitRate : Real


---  
 #  EmitRateSoftStartTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Slowly ramps up to EmitRate over this time.
> ``` lang=cpp, name=Lightning
> var EmitRateSoftStartTime : Real


---  
 #  EmitterSize : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Size of the emitter.
> ``` lang=cpp, name=Lightning
> var EmitterSize : Real3


---  
 #  EmitterVelocityPercent : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much of the objects velocity is added to the particles.
> ``` lang=cpp, name=Lightning
> var EmitterVelocityPercent : Real


---  
 #  EmitVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much the emit can vary per sample.
> ``` lang=cpp, name=Lightning
> var EmitVariance : Real


---  
 #  FastMovingEmitter : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Whether or not we attempt to emit along the vector between the previous position to the current position, which looks better for fast moving particle systems Note: Particle systems that teleport will emit along the teleport line.
> ``` lang=cpp, name=Lightning
> var FastMovingEmitter : Boolean


---  
 #  Fill : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much area of the emitter to used 0 to 1.
> ``` lang=cpp, name=Lightning
> var Fill : Real


---  
 #  Lifetime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How a particle's starting lifetime is.
> ``` lang=cpp, name=Lightning
> var Lifetime : Real


---  
 #  LifetimeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much lifetime can vary per particle.
> ``` lang=cpp, name=Lightning
> var LifetimeVariance : Real


---  
 #  RandomSpin : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Each particle should start with random spin.
> ``` lang=cpp, name=Lightning
> var RandomSpin : Boolean


---  
 #  RandomVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Random Velocity per particle.
> ``` lang=cpp, name=Lightning
> var RandomVelocity : Real3


---  
 #  Size : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Size of each particle spawned.
> ``` lang=cpp, name=Lightning
> var Size : Real


---  
 #  SizeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much the size can vary from the base size per particle.
> ``` lang=cpp, name=Lightning
> var SizeVariance : Real


---  
 #  Spin : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Speed in rads per second of the particle.
> ``` lang=cpp, name=Lightning
> var Spin : Real


---  
 #  SpinVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> How much spin speed can vary per particle.
> ``` lang=cpp, name=Lightning
> var SpinVariance : Real


---  
 #  StartVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Velocity of each particle at start.
> ``` lang=cpp, name=Lightning
> var StartVelocity : Real3


---  
 #  TangentVelocity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

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
 

 
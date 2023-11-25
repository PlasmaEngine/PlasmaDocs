 `Sound`

(NOTE) Plays audio using the specified type of generated wave.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#interpolatedecibels-void)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#decibels-plasma-engine-doc)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
|[ InterpolateVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#interpolatevolume-void)|[ SquareWavePulseValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#squarewavepulsevalue-zer)| | |
|[ InterpolateWaveFrequency](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#interpolatewavefrequency)|[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#volume-plasma-engine-docum)| | |
|[ Play](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#play-void)|[ WaveFrequency](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#wavefrequency-plasma-engin)| | |
|[ Stop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#stop-void)|[ WaveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md#wavetype-plasma-engine-doc)| | |


 #  Properties


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment, in decibels, that will be applied to the sound when it plays. A value of 0 does not affect the sound; 6 will double the sound's volume, -6 will halve it, and -100 is effectively the same as a Volume of 0.
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  SquareWavePulseValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The percentage of the square wave (from 0 to 1.0) which should be up. This will have no effect if a different wave type is chosen.
> ``` lang=cpp, name=Lightning
> var SquareWavePulseValue : Real


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment that will be applied to the sound when it plays. A value of 1 does not affect the sound; 2 will double the sound's volume, 0.5 will halve it, and 0 will make the sound inaudible.
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  WaveFrequency : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The frequency of the generated sound wave. This value will have no effect if the Noise type is chosen.
> ``` lang=cpp, name=Lightning
> var WaveFrequency : Real


---  
 #  WaveType : [SynthWaveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#synthwavetype)

> The type of sound wave used to generate the audio. Possible types are Sine, Square, Saw, Triangle, and Noise (randomly generated white noise).
> ``` lang=cpp, name=Lightning
> var WaveType : SynthWaveType


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateWaveFrequency : Void

> Interpolates the WaveFrequency property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter. This method will have no effect if the Noise type is chosen.
> |Name|Type|Description|
> |---|---|---|
> |frequency|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateWaveFrequency(frequency : Real, time : Real)
> ``` 


---  
 #  Play : Void

> Starts playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Play()
> ``` 


---  
 #  Stop : Void

> Stops playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Stop()
> ``` 


---  
 

 
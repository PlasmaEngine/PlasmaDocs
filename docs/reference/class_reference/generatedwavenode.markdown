 `Sound`

(NOTE) Plays audio using the specified type of generated wave.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#interpolatedecibels-void)|[ Decibels](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#decibels-plasma-engine-doc)|[soundnode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundnode.markdown)| |
|[ InterpolateVolume](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#interpolatevolume-void)|[ SquareWavePulseValue](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#squarewavepulsevalue-zer)| | |
|[ InterpolateWaveFrequency](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#interpolatewavefrequency)|[ Volume](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#volume-plasma-engine-docum)| | |
|[ Play](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#play-void)|[ WaveFrequency](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#wavefrequency-plasma-engin)| | |
|[ Stop](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#stop-void)|[ WaveType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/generatedwavenode.markdown#wavetype-plasma-engine-doc)| | |


 #  Properties


---  
 #  Decibels : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The volume adjustment, in decibels, that will be applied to the sound when it plays. A value of 0 does not affect the sound; 6 will double the sound's volume, -6 will halve it, and -100 is effectively the same as a Volume of 0.
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  SquareWavePulseValue : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The percentage of the square wave (from 0 to 1.0) which should be up. This will have no effect if a different wave type is chosen.
> ``` lang=cpp, name=Lightning
> var SquareWavePulseValue : Real


---  
 #  Volume : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The volume adjustment that will be applied to the sound when it plays. A value of 1 does not affect the sound; 2 will double the sound's volume, 0.5 will halve it, and 0 will make the sound inaudible.
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  WaveFrequency : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The frequency of the generated sound wave. This value will have no effect if the Noise type is chosen.
> ``` lang=cpp, name=Lightning
> var WaveFrequency : Real


---  
 #  WaveType : [SynthWaveType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#synthwavetype)

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
> |decibels|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateWaveFrequency : Void

> Interpolates the WaveFrequency property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter. This method will have no effect if the Noise type is chosen.
> |Name|Type|Description|
> |---|---|---|
> |frequency|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |time|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
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
 

 
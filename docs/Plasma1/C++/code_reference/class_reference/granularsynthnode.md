 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#play-void)|[ BufferScanRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#bufferscanrate-plasma-engi)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
|[ SetSound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#setsound-void)|[ GrainDelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#graindelay-plasma-engine-d)| | |
|[ Stop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#stop-void)|[ GrainDelayVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#graindelayvariance-plasma)| | |
| |[ GrainLength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainlength-plasma-engine)| | |
| |[ GrainLengthVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainlengthvariance-plasma)| | |
| |[ GrainPanningValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainpanningvalue-plasma-e)| | |
| |[ GrainPanningVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainpanningvariance-zer)| | |
| |[ GrainResampleRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainresamplerate-plasma-e)| | |
| |[ GrainResampleRateVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainresampleratevarianc)| | |
| |[ GrainVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainvolume-plasma-engine)| | |
| |[ GrainVolumeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#grainvolumevariance-plasma)| | |
| |[ RandomLocationValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#randomlocationvalue-plasma)| | |
| |[ WindowAttack](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#windowattack-plasma-engine)| | |
| |[ WindowRelease](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#windowrelease-plasma-engin)| | |
| |[ WindowType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md#windowtype-plasma-engine-d)| | |


 #  Properties


---  
 #  BufferScanRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The rate at which the synthesizer scans the buffer as it creates grains. A value of 1.0 will move through the audio data at the same rate as it would normally be played, 0.5 will move at half speed, and -1.0 will move at normal speed backward. A value of 0.0 will make the synthesizer repeat the same audio continuously.
> ``` lang=cpp, name=Lightning
> var BufferScanRate : Real


---  
 #  GrainDelay : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of milliseconds to wait before playing another grain.
> ``` lang=cpp, name=Lightning
> var GrainDelay : Integer


---  
 #  GrainDelayVariance : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The variance for randomizing the grain delay, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainDelayVariance : Integer


---  
 #  GrainLength : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The length of a grain, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainLength : Integer


---  
 #  GrainLengthVariance : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The variance for randomizing the grain length, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainLengthVariance : Integer


---  
 #  GrainPanningValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The value used to pan the grains left or right. A value of 0 will be heard equally from the left and right, 1.0 will be heard only on the right, and -1.0 will be only left.
> ``` lang=cpp, name=Lightning
> var GrainPanningValue : Real


---  
 #  GrainPanningVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The variance for randomizing the grain panning value.
> ``` lang=cpp, name=Lightning
> var GrainPanningVariance : Real


---  
 #  GrainResampleRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The rate at which grains resample their audio data. A value of 1.0 will play normally, 0.5 will play at half speed, and -1.0 will play at normal speed backward. Cannot be 0.
> ``` lang=cpp, name=Lightning
> var GrainResampleRate : Real


---  
 #  GrainResampleRateVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The variance for randomizing the grain resample rate.
> ``` lang=cpp, name=Lightning
> var GrainResampleRateVariance : Real


---  
 #  GrainVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume modifier applied to the grains.
> ``` lang=cpp, name=Lightning
> var GrainVolume : Real


---  
 #  GrainVolumeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The variance for randomizing the grain volume.
> ``` lang=cpp, name=Lightning
> var GrainVolumeVariance : Real


---  
 #  RandomLocationValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The value for controlling how many grains have randomized starting positions in the audio. A value of 0 will be completely sequential, while 1.0 will be completely random.
> ``` lang=cpp, name=Lightning
> var RandomLocationValue : Real


---  
 #  WindowAttack : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The window attack time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Lightning
> var WindowAttack : Integer


---  
 #  WindowRelease : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The window release time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Lightning
> var WindowRelease : Integer


---  
 #  WindowType : [GranularSynthWindows](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#granularsynthwindows)

> The type of window, or volume envelope, used for each grain.
> ``` lang=cpp, name=Lightning
> var WindowType : GranularSynthWindows


---  
 #  Methods


---  
 #  Play : Void

> Starts playing new grains.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Play()
> ``` 


---  
 #  SetSound : Void

> Sets the Sound resource that will be used for the grains, along with an optional start and stop time. If the stopTime is 0.0, all audio from the Sound will be used.
> |Name|Type|Description|
> |---|---|---|
> |sound|[sound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sound.md)| |
> |startTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |stopTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetSound(sound : Sound, startTime : Real, stopTime : Real)
> ``` 


---  
 #  Stop : Void

> Stops playing new grains but continues to play current ones.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Stop()
> ``` 


---  
 

 
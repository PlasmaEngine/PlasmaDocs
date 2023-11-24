 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#play-void)|[ BufferScanRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#bufferscanrate-plasma-engi)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.markdown)| |
|[ SetSound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#setsound-void)|[ GrainDelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#graindelay-plasma-engine-d)| | |
|[ Stop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#stop-void)|[ GrainDelayVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#graindelayvariance-plasma)| | |
| |[ GrainLength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainlength-plasma-engine)| | |
| |[ GrainLengthVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainlengthvariance-plasma)| | |
| |[ GrainPanningValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainpanningvalue-plasma-e)| | |
| |[ GrainPanningVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainpanningvariance-zer)| | |
| |[ GrainResampleRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainresamplerate-plasma-e)| | |
| |[ GrainResampleRateVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainresampleratevarianc)| | |
| |[ GrainVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainvolume-plasma-engine)| | |
| |[ GrainVolumeVariance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#grainvolumevariance-plasma)| | |
| |[ RandomLocationValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#randomlocationvalue-plasma)| | |
| |[ WindowAttack](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#windowattack-plasma-engine)| | |
| |[ WindowRelease](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#windowrelease-plasma-engin)| | |
| |[ WindowType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.markdown#windowtype-plasma-engine-d)| | |


 #  Properties


---  
 #  BufferScanRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The rate at which the synthesizer scans the buffer as it creates grains. A value of 1.0 will move through the audio data at the same rate as it would normally be played, 0.5 will move at half speed, and -1.0 will move at normal speed backward. A value of 0.0 will make the synthesizer repeat the same audio continuously.
> ``` lang=cpp, name=Lightning
> var BufferScanRate : Real


---  
 #  GrainDelay : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The number of milliseconds to wait before playing another grain.
> ``` lang=cpp, name=Lightning
> var GrainDelay : Integer


---  
 #  GrainDelayVariance : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The variance for randomizing the grain delay, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainDelayVariance : Integer


---  
 #  GrainLength : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The length of a grain, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainLength : Integer


---  
 #  GrainLengthVariance : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The variance for randomizing the grain length, in milliseconds.
> ``` lang=cpp, name=Lightning
> var GrainLengthVariance : Integer


---  
 #  GrainPanningValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The value used to pan the grains left or right. A value of 0 will be heard equally from the left and right, 1.0 will be heard only on the right, and -1.0 will be only left.
> ``` lang=cpp, name=Lightning
> var GrainPanningValue : Real


---  
 #  GrainPanningVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The variance for randomizing the grain panning value.
> ``` lang=cpp, name=Lightning
> var GrainPanningVariance : Real


---  
 #  GrainResampleRate : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The rate at which grains resample their audio data. A value of 1.0 will play normally, 0.5 will play at half speed, and -1.0 will play at normal speed backward. Cannot be 0.
> ``` lang=cpp, name=Lightning
> var GrainResampleRate : Real


---  
 #  GrainResampleRateVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The variance for randomizing the grain resample rate.
> ``` lang=cpp, name=Lightning
> var GrainResampleRateVariance : Real


---  
 #  GrainVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume modifier applied to the grains.
> ``` lang=cpp, name=Lightning
> var GrainVolume : Real


---  
 #  GrainVolumeVariance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The variance for randomizing the grain volume.
> ``` lang=cpp, name=Lightning
> var GrainVolumeVariance : Real


---  
 #  RandomLocationValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The value for controlling how many grains have randomized starting positions in the audio. A value of 0 will be completely sequential, while 1.0 will be completely random.
> ``` lang=cpp, name=Lightning
> var RandomLocationValue : Real


---  
 #  WindowAttack : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The window attack time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Lightning
> var WindowAttack : Integer


---  
 #  WindowRelease : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The window release time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Lightning
> var WindowRelease : Integer


---  
 #  WindowType : [GranularSynthWindows](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#granularsynthwindows)

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
> |sound|[sound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sound.markdown)| |
> |startTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |stopTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
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
 

 
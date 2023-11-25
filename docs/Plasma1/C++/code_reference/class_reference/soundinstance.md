 `Sound`

(NOTE) The object associated with a currently playing sound.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#interpolatedecibels-void)|[ CustomEventTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#customeventtime-plasma-eng)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)| |
|[ InterpolatePitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#interpolatepitch-void)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#decibels-plasma-engine-doc)| | |
|[ InterpolateSemitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#interpolatesemitones-voi)|[ EndTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#endtime-plasma-engine-docu)| | |
|[ InterpolateVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#interpolatevolume-void)|[ FileLength](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#filelength-plasma-engine-d)| | |
|[ Stop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#stop-void)|[ IsPlaying](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#isplaying-plasma-engine-do)| | |
| |[ LoopEndTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#loopendtime-plasma-engine)| | |
| |[ Looping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#looping-plasma-engine-docu)| | |
| |[ LoopStartTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#loopstarttime-plasma-engin)| | |
| |[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#paused-plasma-engine-docum)| | |
| |[ Pitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#pitch-plasma-engine-docume)| | |
| |[ Semitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#semitones-plasma-engine-do)| | |
| |[ SoundName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#soundname-plasma-engine-do)| | |
| |[ SoundNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#soundnode-plasma-engine-do)| | |
| |[ Time](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#time-plasma-engine-documen)| | |
| |[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  CustomEventTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time (in seconds from the beginning of the file) to get a MusicCustomTime event.
> ``` lang=cpp, name=Lightning
> var CustomEventTime : Real


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment (in decibels) of the SoundInstance, initially set by the SoundCue's Decibels property. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  EndTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will stop.
> ``` lang=cpp, name=Lightning
> var EndTime : Real


---  
 #  FileLength : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The length of the entire audio file, in seconds.
> ``` lang=cpp, name=Lightning
> var FileLength : Real


---  
 #  IsPlaying : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> This Property will be true while the SoundInstance is playing, then will become false when its sound has stopped.
> ``` lang=cpp, name=Lightning
> var IsPlaying : Boolean


---  
 #  LoopEndTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will stop and jump back when looping.
> ``` lang=cpp, name=Lightning
> var LoopEndTime : Real


---  
 #  Looping : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When this Property is true the SoundInstance will loop indefinitely. If changed to false while a SoundInstance is looping the SoundInstance will continue playing to its EndTime and then stop.
> ``` lang=cpp, name=Lightning
> var Looping : Boolean


---  
 #  LoopStartTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will jump back to when it loops.
> ``` lang=cpp, name=Lightning
> var LoopStartTime : Real


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Setting this Property to true will pause a currently playing SoundInstance. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Pitch : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The pitch adjustment of the SoundInstance, initially set by the SoundCue's Pitch property. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound,.
> ``` lang=cpp, name=Lightning
> var Pitch : Real


---  
 #  Semitones : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The pitch adjustment, in semitones (or half-steps), of the SoundInstance, initially set by the SoundCue's Semitones property. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, and -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Semitones : Real


---  
 #  SoundName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> The name of the Sound being played by this SoundInstance.
> ``` lang=cpp, name=Lightning
> var SoundName : String


---  
 #  SoundNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode associated with this SoundInstance.
> ``` lang=cpp, name=Lightning
> var SoundNode : SoundNode


---  
 #  Time : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> This property tells you to the current playback position, in seconds from the beginning of the file, and allows you to tell the instance to change its playback position to a different time. Be aware that the time will not be precisely accurate. If the Sound resource used to play the SoundInstance has Streamed selected, you cannot set the playback position.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment of the SoundInstance, initially set by the SoundCue's Volume property. A value of 1 does nothing, 2 will double the sound's volume, 0.5 will halve it. The Volume property is linked to the Decibels property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundInstance's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the SoundInstance's Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolatePitch(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the SoundInstance's Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitchSemitones|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateSemitones(pitchSemitones : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundInstance's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  Stop : Void

> Stops the playback of this SoundInstance. It cannot be re-started.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Stop()
> ``` 


---  
 

 
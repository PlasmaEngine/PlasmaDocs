 `Sound`

(NOTE) The object associated with a currently playing sound.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#interpolatedecibels-void)|[ CustomEventTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#customeventtime-plasma-eng)|[referencecountedeventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/referencecountedeventobject.markdown)| |
|[ InterpolatePitch](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#interpolatepitch-void)|[ Decibels](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#decibels-plasma-engine-doc)| | |
|[ InterpolateSemitones](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#interpolatesemitones-voi)|[ EndTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#endtime-plasma-engine-docu)| | |
|[ InterpolateVolume](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#interpolatevolume-void)|[ FileLength](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#filelength-plasma-engine-d)| | |
|[ Stop](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#stop-void)|[ IsPlaying](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#isplaying-plasma-engine-do)| | |
| |[ LoopEndTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#loopendtime-plasma-engine)| | |
| |[ Looping](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#looping-plasma-engine-docu)| | |
| |[ LoopStartTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#loopstarttime-plasma-engin)| | |
| |[ Paused](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#paused-plasma-engine-docum)| | |
| |[ Pitch](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#pitch-plasma-engine-docume)| | |
| |[ Semitones](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#semitones-plasma-engine-do)| | |
| |[ SoundName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#soundname-plasma-engine-do)| | |
| |[ SoundNode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#soundnode-plasma-engine-do)| | |
| |[ Time](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#time-plasma-engine-documen)| | |
| |[ Volume](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  CustomEventTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The time (in seconds from the beginning of the file) to get a MusicCustomTime event.
> ``` lang=cpp, name=Lightning
> var CustomEventTime : Real


---  
 #  Decibels : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The volume adjustment (in decibels) of the SoundInstance, initially set by the SoundCue's Decibels property. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  EndTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The time in seconds from the beginning of the file that the instance will stop.
> ``` lang=cpp, name=Lightning
> var EndTime : Real


---  
 #  FileLength : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The length of the entire audio file, in seconds.
> ``` lang=cpp, name=Lightning
> var FileLength : Real


---  
 #  IsPlaying : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> This Property will be true while the SoundInstance is playing, then will become false when its sound has stopped.
> ``` lang=cpp, name=Lightning
> var IsPlaying : Boolean


---  
 #  LoopEndTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The time in seconds from the beginning of the file that the instance will stop and jump back when looping.
> ``` lang=cpp, name=Lightning
> var LoopEndTime : Real


---  
 #  Looping : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> When this Property is true the SoundInstance will loop indefinitely. If changed to false while a SoundInstance is looping the SoundInstance will continue playing to its EndTime and then stop.
> ``` lang=cpp, name=Lightning
> var Looping : Boolean


---  
 #  LoopStartTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The time in seconds from the beginning of the file that the instance will jump back to when it loops.
> ``` lang=cpp, name=Lightning
> var LoopStartTime : Real


---  
 #  Paused : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Setting this Property to true will pause a currently playing SoundInstance. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Pitch : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The pitch adjustment of the SoundInstance, initially set by the SoundCue's Pitch property. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound,.
> ``` lang=cpp, name=Lightning
> var Pitch : Real


---  
 #  Semitones : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The pitch adjustment, in semitones (or half-steps), of the SoundInstance, initially set by the SoundCue's Semitones property. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, and -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Semitones : Real


---  
 #  SoundName : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The name of the Sound being played by this SoundInstance.
> ``` lang=cpp, name=Lightning
> var SoundName : String


---  
 #  SoundNode : [soundnode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundnode.markdown)

 `read-only`

> The SoundNode associated with this SoundInstance.
> ``` lang=cpp, name=Lightning
> var SoundNode : SoundNode


---  
 #  Time : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> This property tells you to the current playback position, in seconds from the beginning of the file, and allows you to tell the instance to change its playback position to a different time. Be aware that the time will not be precisely accurate. If the Sound resource used to play the SoundInstance has Streamed selected, you cannot set the playback position.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  Volume : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
> |decibels|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the SoundInstance's Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolatePitch(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the SoundInstance's Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitchSemitones|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateSemitones(pitchSemitones : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundInstance's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
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
 

 
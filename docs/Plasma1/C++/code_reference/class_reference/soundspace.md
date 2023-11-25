 `Component` `Sound`



(NOTE) Sound functionality associated with a Space.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#interpolatedecibels-void)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#decibels-plasma-engine-doc)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ InterpolatePitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#interpolatepitch-void)|[ InputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#inputnode-plasma-engine-do)| | |
|[ InterpolateSemitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#interpolatesemitones-voi)|[ MuteAudio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#muteaudio-plasma-engine-do)| | |
|[ InterpolateVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#interpolatevolume-void)|[ OutputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#outputnode-plasma-engine-d)| | |
|[ PlayCue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#playcue-plasma-engine-docu)|[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#paused-plasma-engine-docum)| | |
|[ PlayCuePaused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#playcuepaused-plasma-engin)|[ PauseWithTimeSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#pausewithtimespace-plasma)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#soundspace-void)|[ Pitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#pitch-plasma-engine-docume)| | |
| |[ PitchWithTimeSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#pitchwithtimespace-plasma)| | |
| |[ Semitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#semitones-plasma-engine-do)| | |
| |[ SoundNodeInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#soundnodeinput-plasma-engi)| | |
| |[ SoundNodeOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#soundnodeoutput-plasma-eng)| | |
| |[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundspace.md#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment, in decibels, applied to all sounds in the space. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it.
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  InputNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeInput property should be used instead.
> ``` lang=cpp, name=Lightning
> var InputNode : SoundNode


---  
 #  MuteAudio : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Silences all audio output from this space but processes audio normally.
> ``` lang=cpp, name=Lightning
> var MuteAudio : Boolean


---  
 #  OutputNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeOutput property should be used instead.
> ``` lang=cpp, name=Lightning
> var OutputNode : SoundNode


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Setting this Property to true will pause all audio in the space. Setting it to false will resume all audio.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  PauseWithTimeSpace : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If true, the audio of the space will pause when the space is paused.
> ``` lang=cpp, name=Lightning
> var PauseWithTimeSpace : Boolean


---  
 #  Pitch : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The pitch adjustment applied to all sounds in the space. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound, -1 will lower the sound by an octave and slow it down.
> ``` lang=cpp, name=Lightning
> var Pitch : Real


---  
 #  PitchWithTimeSpace : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If true, the audio in the SoundSpace will be pitched according to the TimeScale of the Space(if time slows down the audio will slow down and lower in pitch, if it speeds up the audio will speed up and raise in pitch).
> ``` lang=cpp, name=Lightning
> var PitchWithTimeSpace : Boolean


---  
 #  Semitones : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The pitch adjustment, in semitones (or half-steps), applied to all sounds in the space. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound,.
> ``` lang=cpp, name=Lightning
> var Semitones : Real


---  
 #  SoundNodeInput : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode which is the ultimate output of all sounds in this space.
> ``` lang=cpp, name=Lightning
> var SoundNodeInput : SoundNode


---  
 #  SoundNodeOutput : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode which can be used to attach other nodes which should process all audio in the SoundSpace.
> ``` lang=cpp, name=Lightning
> var SoundNodeOutput : SoundNode


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment applied to all sounds in the space. A value of 1 does nothing, 2 will double the volume, 0.5 will halve it.
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundSpace's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the SoundSpace's Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolatePitch(pitch : Real, time : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the SoundSpace's Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateSemitones(pitch : Real, time : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundSpace's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolume(value : Real, interpolationTime : Real)
> ``` 


---  
 #  PlayCue : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

> Plays the passed-in SoundCue non-positionally and returns the resulting SoundInstance.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md)| |
> ``` lang=cpp, name=Lightning
> function PlayCue(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  PlayCuePaused : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

> Plays the passed-in SoundCue non-positionally and returns the resulting SoundInstance, which starts off paused.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md)| |
> ``` lang=cpp, name=Lightning
> function PlayCuePaused(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  SoundSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SoundSpace()
> ``` 


---  
 

 
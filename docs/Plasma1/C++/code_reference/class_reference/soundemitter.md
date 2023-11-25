 `Component` `Sound`



(NOTE) Allows 3D positioning of sounds relative to SoundListeners.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#interpolatedecibels-void)|[ Attenuator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#attenuator-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ InterpolatePitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#interpolatepitch-void)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#decibels-plasma-engine-doc)| | |
|[ InterpolateSemitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#interpolatesemitones-voi)|[ Directional](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#directional-plasma-engine)| | |
|[ InterpolateVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#interpolatevolume-void)|[ EmitAngle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#emitangle-plasma-engine-do)| | |
|[ PlayCue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#playcue-plasma-engine-docu)|[ InputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#inputnode-plasma-engine-do)| | |
|[ PlayCuePaused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#playcuepaused-plasma-engin)|[ IsPlaying](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#isplaying-plasma-engine-do)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#soundemitter-void)|[ OutputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#outputnode-plasma-engine-d)| | |
| |[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#paused-plasma-engine-docum)| | |
| |[ Pitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#pitch-plasma-engine-docume)| | |
| |[ RearVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#rearvolume-plasma-engine-d)| | |
| |[ Semitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#semitones-plasma-engine-do)| | |
| |[ SoundNodeInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#soundnodeinput-plasma-engi)| | |
| |[ SoundNodeOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#soundnodeoutput-plasma-eng)| | |
| |[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundemitter.md#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  Attenuator : [soundattenuator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.md)

> If a SoundAttenuator resource other than DefaultNoAttenuation is selected it will be applied to SoundCues without their own SoundAttenuator resource. If a SoundCue has attenuation settings those will always be used. If neither has settings, the sound will not be attenuated.
> ``` lang=cpp, name=Lightning
> var Attenuator : SoundAttenuator


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment, in decibels, applied to all sounds played through this SoundEmitter. A value of 0 does nothing, 6 will double the volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  Directional : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When true, the audio output of the SoundEmitter will be limited by the EmitAngle, so that sound in front of the object will be louder than sound behind it. Within the EmitAngle the sound will be at full volume. The volume interpolates logarithmically until it reaches the RearVolume value directly behind the object.
> ``` lang=cpp, name=Lightning
> var Directional : Boolean


---  
 #  EmitAngle : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The angle of full volume sound for a directional SoundEmitter, from 1 to 360. An angle of 90, for example, will be centered at the object's front, extending 45 degrees to the left and right.
> ``` lang=cpp, name=Lightning
> var EmitAngle : Real


---  
 #  InputNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeInput property should be used instead.
> ``` lang=cpp, name=Lightning
> var InputNode : SoundNode


---  
 #  IsPlaying : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> This property will be true if there are SoundInstances currently associated with this SoundEmitter, even if they are paused or otherwise not audible.
> ``` lang=cpp, name=Lightning
> var IsPlaying : Boolean


---  
 #  OutputNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeOutput property should be used instead.
> ``` lang=cpp, name=Lightning
> var OutputNode : SoundNode


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Setting this property to true pauses all sounds currently playing through the SoundEmitter. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Pitch : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> This property affects both the pitch and speed of all sounds played through this SoundEmitter. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound, -1 will lower the sound by an octave and slow it down. The Pitch property is linked to the Semitones property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Pitch : Real


---  
 #  RearVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume of sound heard directly behind a directional SoundEmitter. It will only reach this value in a small area, since volume is interpolated from the edge of the EmitAngle. To make the volume as quiet as possible behind the object, use a small EmitAngle.
> ``` lang=cpp, name=Lightning
> var RearVolume : Real


---  
 #  Semitones : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> This property, specified in semitones (or half-steps), affects both the pitch and speed of all sounds played through this SoundEmitter.. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Semitones : Real


---  
 #  SoundNodeInput : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode to use for attaching other nodes to the input of the SoundEmitter.
> ``` lang=cpp, name=Lightning
> var SoundNodeInput : SoundNode


---  
 #  SoundNodeOutput : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode to use for attaching other nodes to the output of the SoundEmitter.
> ``` lang=cpp, name=Lightning
> var SoundNodeOutput : SoundNode


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment applied to all sounds played through this SoundEmitter. A value of 1 does nothing, 2 will double the volume, 0.5 will halve it. The Volume property is linked to the Decibels property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Volume : Real


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
 #  InterpolatePitch : Void

> Interpolates the Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolatePitch(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateSemitones(pitch : Real, interpolationTime : Real)
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
 #  PlayCue : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

> Plays the SoundCue passed into the function and returns the resulting SoundInstance.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md)| |
> ``` lang=cpp, name=Lightning
> function PlayCue(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  PlayCuePaused : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

> Plays the SoundCue passed into the function and returns the resulting SoundInstance, which starts off paused.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md)| |
> ``` lang=cpp, name=Lightning
> function PlayCuePaused(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  SoundEmitter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SoundEmitter()
> ``` 


---  
 

 
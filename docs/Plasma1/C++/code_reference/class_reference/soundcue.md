 `Resource` `Sound`



(NOTE) Settings and Sounds for playing audio files.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddSoundEntry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#addsoundentry-void)|[ Attenuator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#attenuator-plasma-engine-d)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
|[ AddSoundTagEntry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#addsoundtagentry-void)|[ BeatsPerMinute](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#beatsperminute-plasma-engi)| | |
|[ PlayCueOnNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#playcueonnode-plasma-engin)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#decibels-plasma-engine-doc)| | |
|[ Preview](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#preview-void)|[ DecibelVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#decibelvariation-plasma-en)| | |
|[ StopPreview](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#stoppreview-void)|[ Pitch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#pitch-plasma-engine-docume)| | |
| |[ PitchVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#pitchvariation-plasma-engi)| | |
| |[ PlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#playmode-plasma-engine-doc)| | |
| |[ SelectMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#selectmode-plasma-engine-d)| | |
| |[ Semitones](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#semitones-plasma-engine-do)| | |
| |[ SemitoneVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#semitonevariation-plasma-e)| | |
| |[ ShowMusicOptions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#showmusicoptions-plasma-en)| | |
| |[ Sounds](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#sounds-plasma-engine-docum)| | |
| |[ SoundTags](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#soundtags-plasma-engine-do)| | |
| |[ TimeSigBeats](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#timesigbeats-plasma-engine)| | |
| |[ TimeSigValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#timesigvalue-plasma-engine)| | |
| |[ UseDecibelVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#usedecibelvariation-plasma)| | |
| |[ UseSemitoneVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#usesemitonevariation-zer)| | |
| |[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#volume-plasma-engine-docum)| | |
| |[ VolumeVariation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md#volumevariation-plasma-eng)| | |


 #  Properties


---  
 #  Attenuator : [soundattenuator](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.md)

> If a SoundAttenuator resource is selected, it will be applied to reduce the sound's volume with distance when played through a SoundEmitter. If DefaultNoAttenuation is selected on the SoundCue and a different SoundAttenuator is selected on the SoundEmitter, the SoundEmitter's settings will be applied. If DefaultNoAttenuation is selected on both the sound will not be attenuated.
> ``` lang=cpp, name=Lightning
> var Attenuator : SoundAttenuator


---  
 #  BeatsPerMinute : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The speed of the music, using beats per minute.
> ``` lang=cpp, name=Lightning
> var BeatsPerMinute : Real


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment, in decibels, that will be applied to the sound when it plays. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  DecibelVariation : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Sets how much the Decibels will be randomized every time the SoundCue plays. If Decibels is 0, and DecibelVariation is 4, the volume adjustment will be chosen randomly between -4 and 4.
> ``` lang=cpp, name=Lightning
> var DecibelVariation : Real


---  
 #  Pitch : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> This property affects both the pitch and speed of the sound played by the SoundCue. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound,.
> ``` lang=cpp, name=Lightning
> var Pitch : Real


---  
 #  PitchVariation : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Sets how much the pitch will be randomized every time the SoundCue plays. If Pitch is 0, and PitchVariation is 0.3, the pitch of the sound will be chosen randomly between -0.3 and 0.3.
> ``` lang=cpp, name=Lightning
> var PitchVariation : Real


---  
 #  PlayMode : [SoundPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#soundplaymode)

> If Single is chosen the SoundInstance created by the SoundCue will be played once and will stop when it reaches its EndTime. If Looping is chosen the SoundInstance will play continuously until either it is stopped or its Looping property is set to false.
> ``` lang=cpp, name=Lightning
> var PlayMode : SoundPlayMode


---  
 #  SelectMode : [SoundSelectMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#soundselectmode)

> If Random is chosen the SoundCue will randomly choose which SoundEntry to play. If Sequential is chosen it will play the SoundEntries in order.
> ``` lang=cpp, name=Lightning
> var SelectMode : SoundSelectMode


---  
 #  Semitones : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> This property, specified in semitones (or half-steps), affects both the pitch and speed of the sound played by the SoundCue. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, and -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Semitones : Real


---  
 #  SemitoneVariation : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Sets how much the pitch will be randomized every time the SoundCue plays. If Semitones is 0, and SemitoneVariation is 5, the pitch of the sound will be chosen randomly between -5 and 5.
> ``` lang=cpp, name=Lightning
> var SemitoneVariation : Real


---  
 #  ShowMusicOptions : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If true, the music options will be shown. If false, they will be hidden.
> ``` lang=cpp, name=Lightning
> var ShowMusicOptions : Boolean


---  
 #  Sounds : [sounds](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sounds.md)

> 
> ``` lang=cpp, name=Lightning
> var Sounds : Sounds


---  
 #  SoundTags : [soundtags](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtags.md)

> 
> ``` lang=cpp, name=Lightning
> var SoundTags : SoundTags


---  
 #  TimeSigBeats : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The top number of the music's time signature (beats per measure).
> ``` lang=cpp, name=Lightning
> var TimeSigBeats : Real


---  
 #  TimeSigValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The bottom number of the music's time signature (which type of note has the beat).
> ``` lang=cpp, name=Lightning
> var TimeSigValue : Real


---  
 #  UseDecibelVariation : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If false, the VolumeVariation value will be used to randomize the volume. If true, the DecibelVariation field will be shown and will be used for randomization.
> ``` lang=cpp, name=Lightning
> var UseDecibelVariation : Boolean


---  
 #  UseSemitoneVariation : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If false, the PitchVariation value will be used to randomize the volume. If true, the SemitoneVariation field will be shown and will be used for randomization.
> ``` lang=cpp, name=Lightning
> var UseSemitoneVariation : Boolean


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment that will be applied to the sound when it plays. A value of 1 does nothing, 2 will double the sound's volume, 0.5 will halve it. The Volume property is linked to the Decibels property (changing one will change the other).
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  VolumeVariation : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Sets how much the Volume will be randomized every time the SoundCue plays. If Volume is 1, and VolumeVariation is 0.5, the volume adjustment will be chosen randomly between 0.5 and 1.5.
> ``` lang=cpp, name=Lightning
> var VolumeVariation : Real


---  
 #  Methods


---  
 #  AddSoundEntry : Void

> Adds a new SoundEntry to this SoundCue.
> |Name|Type|Description|
> |---|---|---|
> |sound|[sound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sound.md)| |
> |weight|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function AddSoundEntry(sound : Sound, weight : Real)
> ``` 


---  
 #  AddSoundTagEntry : Void

> Adds a new SoundTagEntry to this SoundCue.
> |Name|Type|Description|
> |---|---|---|
> |soundTag|[soundtag](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.md)| |
> ``` lang=cpp, name=Lightning
> function AddSoundTagEntry(soundTag : SoundTag)
> ``` 


---  
 #  PlayCueOnNode : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

> Plays this SoundCue using a specified SoundNode as the output and returns the resulting SoundInstance.
> |Name|Type|Description|
> |---|---|---|
> |outputNode|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> |startPaused|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function PlayCueOnNode(outputNode : SoundNode, startPaused : Boolean) : SoundInstance
> ``` 


---  
 #  Preview : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Preview()
> ``` 


---  
 #  StopPreview : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StopPreview()
> ``` 


---  
 

 
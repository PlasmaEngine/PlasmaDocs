 `Sound`

(NOTE) Stores Sounds and associated properties to be used by a SoundCue.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Preview](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#preview-void)|[ CrossFadeLoopTail](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#crossfadelooptail-plasma-e)|Object| |
|[ StopPreview](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#stoppreview-void)|[ EndTime](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#endtime-plasma-engine-docu)| | |
| |[ LoopEndTime](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#loopendtime-plasma-engine)| | |
| |[ LoopStartTime](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#loopstarttime-plasma-engin)| | |
| |[ LoopTailLength](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#looptaillength-plasma-engi)| | |
| |[ Sound](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#sound-plasma-engine-docume)| | |
| |[ StartTime](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#starttime-plasma-engine-do)| | |
| |[ Weight](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundentry.markdown#weight-plasma-engine-docum)| | |


 #  Properties


---  
 #  CrossFadeLoopTail : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> If false, the loop tail will be added to the audio and will fade out over the specified time. If true, the audio will be cross-faded, so the beginning of the loop will fade in as the tail fades out.
> ``` lang=cpp, name=Lightning
> var CrossFadeLoopTail : Boolean


---  
 #  EndTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The time (in seconds) at which the Sound will stop playing. Defaults to the length of the audio file. Cannot be smaller than the StartTime.
> ``` lang=cpp, name=Lightning
> var EndTime : Real


---  
 #  LoopEndTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The time (in seconds) from the beginning of the audio file at which a looping SoundInstance jumps back to the LoopStartTime. If it stops looping while playing it will continue to the EndTime and then stop. Cannot be smaller than the LoopStartTime.
> ``` lang=cpp, name=Lightning
> var LoopEndTime : Real


---  
 #  LoopStartTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The time (in seconds) from the beginning of the audio file that a looping SoundInstance will jump back to after it reaches the LoopEndTime. The Sound will still start at the StartTime when it is played, but after it begins looping it will start at the LoopStartTime. Cannot be larger than the LoopEndTime.
> ``` lang=cpp, name=Lightning
> var LoopStartTime : Real


---  
 #  LoopTailLength : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The length (in seconds) of the tail, from the LoopEndTime, which will continue to play after the Sound jumps back to the LoopStartTime. The loop tail will fade out smoothly.
> ``` lang=cpp, name=Lightning
> var LoopTailLength : Real


---  
 #  Sound : [sound](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sound.markdown)

> The Sound resource that will be played by this SoundEntry.
> ``` lang=cpp, name=Lightning
> var Sound : Sound


---  
 #  StartTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The time (in seconds) at which the Sound will start playing. A value of 0 will start the Sound at the beginning of the audio file. Cannot be larger than the EndTime.
> ``` lang=cpp, name=Lightning
> var StartTime : Real


---  
 #  Weight : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The weighted randomization value for this particular SoundEntry to be chosen to play. The values of all SoundEntries are considered: two SoundEntries with weights of 1 and 1 will each play 50 percent of the time, as will weights of 10 and 10.
> ``` lang=cpp, name=Lightning
> var Weight : Real


---  
 #  Methods


---  
 #  Preview : Void

> Preview this sound with no SoundCue settings.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Preview()
> ``` 


---  
 #  StopPreview : Void

> Stop previewing this sound.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StopPreview()
> ``` 


---  
 

 
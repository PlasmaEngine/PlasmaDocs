 `Component` `Sound`



(NOTE) Plays a specified SoundCue, either when created or when the Play method is called.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#play-plasma-engine-documen)|[ Cue](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#cue-plasma-engine-document)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#simplesound-void)|[ IsPlaying](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#isplaying-plasma-engine-do)| | |
|[ Stop](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#stop-void)|[ Paused](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#paused-plasma-engine-docum)| | |
| |[ Positional](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#positional-plasma-engine-d)| | |
| |[ StartPlaying](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/simplesound.markdown#startplaying-plasma-engine)| | |


 #  Properties


---  
 #  Cue : [soundcue](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundcue.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Cue : SoundCue


---  
 #  IsPlaying : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Will be true if the SoundCue is currently being played.
> ``` lang=cpp, name=Lightning
> var IsPlaying : Boolean


---  
 #  Paused : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Setting this Property to true will pause a currently playing SoundCue. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Positional : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If this property is true the SoundCue will be played positionally (heard at a specific location by SoundListeners) through the SoundEmitter component on the same object. If false, the SoundCue will be played through the SoundSpace, and will NOT be affected by any SoundEmitter settings.
> ``` lang=cpp, name=Lightning
> var Positional : Boolean


---  
 #  StartPlaying : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If this property is true the SoundCue will begin playing as soon as the object is created.
> ``` lang=cpp, name=Lightning
> var StartPlaying : Boolean


---  
 #  Methods


---  
 #  Play : [soundinstance](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/soundinstance.markdown)

> Begins playing the SoundCue chosen in the Cue property and returns the resulting SoundInstance. If already playing it will be stopped and re-started.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Play() : SoundInstance
> ``` 


---  
 #  SimpleSound : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SimpleSound()
> ``` 


---  
 #  Stop : Void

> Stops a currently playing SoundInstance if it exists.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Stop()
> ``` 


---  
 

 
 `Component` `Sound`



(NOTE) Plays a specified SoundCue, either when created or when the Play method is called.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#play-plasma-engine-documen)|[ Cue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#cue-plasma-engine-document)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#simplesound-void)|[ IsPlaying](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#isplaying-plasma-engine-do)| | |
|[ Stop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#stop-void)|[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#paused-plasma-engine-docum)| | |
| |[ Positional](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#positional-plasma-engine-d)| | |
| |[ StartPlaying](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplesound.md#startplaying-plasma-engine)| | |


 #  Properties


---  
 #  Cue : [soundcue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundcue.md)

> 
> ``` lang=cpp, name=Lightning
> var Cue : SoundCue


---  
 #  IsPlaying : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Will be true if the SoundCue is currently being played.
> ``` lang=cpp, name=Lightning
> var IsPlaying : Boolean


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Setting this Property to true will pause a currently playing SoundCue. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Positional : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If this property is true the SoundCue will be played positionally (heard at a specific location by SoundListeners) through the SoundEmitter component on the same object. If false, the SoundCue will be played through the SoundSpace, and will NOT be affected by any SoundEmitter settings.
> ``` lang=cpp, name=Lightning
> var Positional : Boolean


---  
 #  StartPlaying : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If this property is true the SoundCue will begin playing as soon as the object is created.
> ``` lang=cpp, name=Lightning
> var StartPlaying : Boolean


---  
 #  Methods


---  
 #  Play : [soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.md)

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
 

 
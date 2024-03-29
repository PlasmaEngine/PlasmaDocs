 `Sound`

(NOTE) Saves audio from its input SoundNodes and then plays it. All audio from inputs is passed to outputs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearSavedAudio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/saveaudionode.md#clearsavedaudio-void)|[ SaveAudio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/saveaudionode.md#saveaudio-plasma-engine-do)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
|[ PlaySavedAudio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/saveaudionode.md#playsavedaudio-void)| | | |
|[ StopPlaying](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/saveaudionode.md#stopplaying-void)| | | |


 #  Properties


---  
 #  SaveAudio : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When true, audio from input SoundNodes will be saved. Setting this to true will remove any existing saved audio before saving more.
> ``` lang=cpp, name=Lightning
> var SaveAudio : Boolean


---  
 #  Methods


---  
 #  ClearSavedAudio : Void

> Removes all currently saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearSavedAudio()
> ``` 


---  
 #  PlaySavedAudio : Void

> Plays the saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PlaySavedAudio()
> ``` 


---  
 #  StopPlaying : Void

> Stops playing the saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StopPlaying()
> ``` 


---  
 

 
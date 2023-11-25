 `Component` `Sound`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#audiosettings-void)|[ LatencySetting](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#latencysetting-plasma-engi)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ MinVolumeThreshold](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#minvolumethreshold-plasma)| | |
| |[ MixType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#mixtype-plasma-engine-docu)| | |
| |[ MuteAllAudio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#muteallaudio-plasma-engine)| | |
| |[ SystemVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audiosettings.md#systemvolume-plasma-engine)| | |


 #  Properties


---  
 #  LatencySetting : [AudioLatency](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#audiolatency)

> Using the high latency setting can fix some audio problems (such as clicks and static) but can lead to a slight delay in the audio.
> ``` lang=cpp, name=Lightning
> var LatencySetting : AudioLatency


---  
 #  MinVolumeThreshold : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Sets the volume threshold at which sounds will be virtualized (they will continue tracking their position and all data but will not process audio). This is a floating point volume number, not decibels.
> ``` lang=cpp, name=Lightning
> var MinVolumeThreshold : Real


---  
 #  MixType : [AudioMixTypes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#audiomixtypes)

> Sets the number of channels the audio system uses when creating audio. See the enum descriptions. If your selection is different from the output device, it will be automatically translated to match the number of channels needed for output.
> ``` lang=cpp, name=Lightning
> var MixType : AudioMixTypes


---  
 #  MuteAllAudio : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> When true, audio will be processed normally but will be silent.
> ``` lang=cpp, name=Lightning
> var MuteAllAudio : Boolean


---  
 #  SystemVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> An overall volume modifier that is applied to all audio produced by Plasma.
> ``` lang=cpp, name=Lightning
> var SystemVolume : Real


---  
 #  Methods


---  
 #  AudioSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AudioSettings()
> ``` 


---  
 

 
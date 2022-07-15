 `Component` `Sound`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#audiosettings-void)|[ LatencySetting](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#latencysetting-plasma-engi)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |
| |[ MinVolumeThreshold](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#minvolumethreshold-plasma)| | |
| |[ MixType](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#mixtype-plasma-engine-docu)| | |
| |[ MuteAllAudio](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#muteallaudio-plasma-engine)| | |
| |[ SystemVolume](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/audiosettings.markdown#systemvolume-plasma-engine)| | |


 #  Properties


---  
 #  LatencySetting : [AudioLatency](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#audiolatency)

> Using the high latency setting can fix some audio problems (such as clicks and static) but can lead to a slight delay in the audio.
> ``` lang=cpp, name=Lightning
> var LatencySetting : AudioLatency


---  
 #  MinVolumeThreshold : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> Sets the volume threshold at which sounds will be virtualized (they will continue tracking their position and all data but will not process audio). This is a floating point volume number, not decibels.
> ``` lang=cpp, name=Lightning
> var MinVolumeThreshold : Real


---  
 #  MixType : [AudioMixTypes](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#audiomixtypes)

> Sets the number of channels the audio system uses when creating audio. See the enum descriptions. If your selection is different from the output device, it will be automatically translated to match the number of channels needed for output.
> ``` lang=cpp, name=Lightning
> var MixType : AudioMixTypes


---  
 #  MuteAllAudio : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> When true, audio will be processed normally but will be silent.
> ``` lang=cpp, name=Lightning
> var MuteAllAudio : Boolean


---  
 #  SystemVolume : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

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
 

 
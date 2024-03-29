 `Sound`

(NOTE) Changes the left and right channel volumes of its input SoundNode's audio separately.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateLeftVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#interpolateleftvolume-vo)|[ LeftVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#leftvolume-plasma-engine-d)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
|[ InterpolateRightVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#interpolaterightvolume-v)|[ RightVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#rightvolume-plasma-engine)| | |
|[ InterpolateVolumes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#interpolatevolumes-void)|[ SumToMono](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md#sumtomono-plasma-engine-do)| | |


 #  Properties


---  
 #  LeftVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume multiplier applied to audio in the left channel.
> ``` lang=cpp, name=Lightning
> var LeftVolume : Real


---  
 #  RightVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume multiplier applied to audio in the right channel.
> ``` lang=cpp, name=Lightning
> var RightVolume : Real


---  
 #  SumToMono : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If this property is true, the audio will be combined into a single channel before being split between the right and left channels. If it is false and the audio has more than two channels, it will be combined into only two channels before being processed.
> ``` lang=cpp, name=Lightning
> var SumToMono : Boolean


---  
 #  Methods


---  
 #  InterpolateLeftVolume : Void

> Interpolates the LeftVolume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateLeftVolume(volume : Real, time : Real)
> ``` 


---  
 #  InterpolateRightVolume : Void

> Interpolates the RightVolume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateRightVolume(volume : Real, time : Real)
> ``` 


---  
 #  InterpolateVolumes : Void

> Interpolates both left and right volume properties at once. The first parameter is the value to change the LeftVolume to, the second is the RightVolume, and the third is the number of seconds to use for the interpolation.
> |Name|Type|Description|
> |---|---|---|
> |leftVolume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |rightVolume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolumes(leftVolume : Real, rightVolume : Real, time : Real)
> ``` 


---  
 

 
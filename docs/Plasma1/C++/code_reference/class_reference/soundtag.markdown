 `Resource` `Sound`



(NOTE) Controls settings on all tagged SoundInstances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ EQSetAllBands](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqsetallbands-void)|[ CompressorAttack](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#compressorattack-plasma-en)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.markdown)| |
|[ InterpolateDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#interpolatedecibels-void)|[ CompressorKneeWidth](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#compressorkneewidth-plasma)| | |
|[ InterpolateVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#interpolatevolume-void)|[ CompressorRatio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#compressorratio-plasma-eng)| | |
|[ StopSounds](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#stopsounds-void)|[ CompressorRelease](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#compressorrelease-plasma-e)| | |
|[ TagSound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#tagsound-void)|[ CompressorThreshold](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#compressorthreshold-plasma)| | |
|[ UnTagSound](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#untagsound-void)|[ Decibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#decibels-plasma-engine-doc)| | |
| |[ EQBand1Gain](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqband1gain-plasma-engine)| | |
| |[ EQBand2Gain](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqband2gain-plasma-engine)| | |
| |[ EQBand3Gain](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqband3gain-plasma-engine)| | |
| |[ EQHighPassGain](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqhighpassgain-plasma-engi)| | |
| |[ EQLowPassGain](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#eqlowpassgain-plasma-engin)| | |
| |[ InstanceCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#instancecount-plasma-engin)| | |
| |[ InstanceLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#instancelimit-plasma-engin)| | |
| |[ Instances](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#instances-plasma-engine-do)| | |
| |[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#paused-plasma-engine-docum)| | |
| |[ TagForDucking](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#tagforducking-plasma-engin)| | |
| |[ UseCompressor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#usecompressor-plasma-engin)| | |
| |[ UseEqualizer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#useequalizer-plasma-engine)| | |
| |[ Volume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown#volume-plasma-engine-docum)| | |


 #  Properties


---  
 #  CompressorAttack : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The time, in milliseconds, for the filter to ramp to full effect after the input reaches the threshold.
> ``` lang=cpp, name=Lightning
> var CompressorAttack : Real


---  
 #  CompressorKneeWidth : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The knee width of the filter, in decibels.
> ``` lang=cpp, name=Lightning
> var CompressorKneeWidth : Real


---  
 #  CompressorRatio : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The ratio of the compression applied by the filter.
> ``` lang=cpp, name=Lightning
> var CompressorRatio : Real


---  
 #  CompressorRelease : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The time, in milliseconds, for the filter to ramp from full effect to off after the input drops below the threshold.
> ``` lang=cpp, name=Lightning
> var CompressorRelease : Real


---  
 #  CompressorThreshold : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The threshold, in decibels, at which the volume is affected by the filter.
> ``` lang=cpp, name=Lightning
> var CompressorThreshold : Real


---  
 #  Decibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment, in decibels, applied to all tagged instances.
> ``` lang=cpp, name=Lightning
> var Decibels : Real


---  
 #  EQBand1Gain : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to frequencies within the band centered at 150 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Lightning
> var EQBand1Gain : Real


---  
 #  EQBand2Gain : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to frequencies within the band centered at 600 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Lightning
> var EQBand2Gain : Real


---  
 #  EQBand3Gain : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to frequencies within the band centered at 2500 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Lightning
> var EQBand3Gain : Real


---  
 #  EQHighPassGain : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to frequencies above 5000 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Lightning
> var EQHighPassGain : Real


---  
 #  EQLowPassGain : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to frequencies below 80 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Lightning
> var EQLowPassGain : Real


---  
 #  InstanceCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> The number of SoundInstances currently associated with this SoundTag.
> ``` lang=cpp, name=Lightning
> var InstanceCount : Integer


---  
 #  InstanceLimit : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> If this value is greater than plasma, SoundCues with this SoundTag will only play if the number of tagged SoundInstances is less than this number.
> ``` lang=cpp, name=Lightning
> var InstanceLimit : Real


---  
 #  Instances : [soundinstancerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstancerange.markdown)

 `read-only`

> This allows you to get all currently tagged SoundInstances. Using a foreach loop, you can access any SoundInstance functionality on each of the tagged instances.
> ``` lang=cpp, name=Lightning
> var Instances : SoundInstanceRange


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Setting this property to true will pause all tagged instances. Setting it to false will resume playback.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  TagForDucking : [soundtag](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundtag.markdown)

> If this property is not null, the selected SoundTag will be used to trigger this SoundTag's compressor.
> ``` lang=cpp, name=Lightning
> var TagForDucking : SoundTag


---  
 #  UseCompressor : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If true, the SoundTag's compressor settings will be applied to the tagged SoundInstances.
> ``` lang=cpp, name=Lightning
> var UseCompressor : Boolean


---  
 #  UseEqualizer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If true, the SoundTag's equalizer settings will be applied to the tagged SoundInstances.
> ``` lang=cpp, name=Lightning
> var UseEqualizer : Boolean


---  
 #  Volume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The volume adjustment applied to all tagged instances.
> ``` lang=cpp, name=Lightning
> var Volume : Real


---  
 #  Methods


---  
 #  EQSetAllBands : Void

> Sets all equalizer band gain values at once. The parameters are in order from the lowest band to the highest. The last parameter is the number of seconds to interpolate the values over.
> |Name|Type|Description|
> |---|---|---|
> |lowPass|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |band1|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |band2|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |band3|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |highPass|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |timeToInterpolate|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function EQSetAllBands(lowPass : Real, band1 : Real, band2 : Real, band3 : Real, highPass : Real, timeToInterpolate : Real)
> ``` 


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundTag's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundTag's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |interpolationTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function InterpolateVolume(value : Real, interpolationTime : Real)
> ``` 


---  
 #  StopSounds : Void

> Stops all currently tagged SoundInstances.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StopSounds()
> ``` 


---  
 #  TagSound : Void

> Adds a new SoundInstance to this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.markdown)| |
> ``` lang=cpp, name=Lightning
> function TagSound(instance : SoundInstance)
> ``` 


---  
 #  UnTagSound : Void

> Removes a SoundInstance from this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundinstance.markdown)| |
> ``` lang=cpp, name=Lightning
> function UnTagSound(instance : SoundInstance)
> ``` 


---  
 

 
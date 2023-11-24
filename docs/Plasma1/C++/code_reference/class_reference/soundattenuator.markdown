 `Resource` `Sound`



(NOTE) Decreases a positional sound's volume as the SoundEmitter gets further away from a SoundListener.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FalloffCurve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#falloffcurve-plasma-engine)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.markdown)| |
| |[ FalloffCurveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#falloffcurvetype-plasma-en)| | |
| |[ LowPassCutoffFreq](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#lowpasscutofffreq-plasma-e)| | |
| |[ LowPassStartDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#lowpassstartdistance-zer)| | |
| |[ MinAttenuatedVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#minattenuatedvolume-plasma)| | |
| |[ StartDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#startdistance-plasma-engin)| | |
| |[ StopDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#stopdistance-plasma-engine)| | |
| |[ UseLowPassFilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown#uselowpassfilter-plasma-en)| | |


 #  Properties


---  
 #  FalloffCurve : [samplecurve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/samplecurve.markdown)

> The SampleCurve resource to use as the attenuation's falloff curve. It will be normalized and stretched to fit between the StartDistance and StopDistance values.
> ``` lang=cpp, name=Lightning
> var FalloffCurve : SampleCurve


---  
 #  FalloffCurveType : [FalloffCurveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#falloffcurvetype)

> The type of curve used to reduce the sound's volume over distance. The default is a logarithmic curve which mimics the real world.
> ``` lang=cpp, name=Lightning
> var FalloffCurveType : FalloffCurveType


---  
 #  LowPassCutoffFreq : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The lowest cutoff frequency of the low pass filter, reached at the StopDistance. The cutoff frequency will be interpolated logarithmically from 15000.00 (a value with very little effect on the sound) to the LowPassCutoffFreq between the LowPassStartDistance and the StopDistance.
> ``` lang=cpp, name=Lightning
> var LowPassCutoffFreq : Real


---  
 #  LowPassStartDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The distance at which the low pass filter begins to take effect.
> ``` lang=cpp, name=Lightning
> var LowPassStartDistance : Real


---  
 #  MinAttenuatedVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The lowest volume that the attenuation will reach. If set above 0, the sound will continue to be heard at all distances.
> ``` lang=cpp, name=Lightning
> var MinAttenuatedVolume : Real


---  
 #  StartDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The distance from a SoundListener at which the sound's volume begins attenuating. At shorter distances the volume will not be changed. Cannot be larger than the StopDistance.
> ``` lang=cpp, name=Lightning
> var StartDistance : Real


---  
 #  StopDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The distance at which the attenuation reaches the minimum volume. No volume changes will happen past this distance. Cannot be smaller than the StartDistance.
> ``` lang=cpp, name=Lightning
> var StopDistance : Real


---  
 #  UseLowPassFilter : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If true, a low pass filter will be applied to the sound after reaching a specified distance, mimicking the way sound is muffled with distance in real life. The filter begins at the LowPassStartDistance and interpolates its cutoff frequency logarithmically until the StopDistance. The filter will not change past the StopDistance.
> ``` lang=cpp, name=Lightning
> var UseLowPassFilter : Boolean


---  
 #  Methods


---  
 

 
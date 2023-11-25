 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AttackMillisec](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#attackmillisec-plasma-engi)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
| |[ InputGainDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#inputgaindecibels-plasma-e)| | |
| |[ KneeWidth](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#kneewidth-plasma-engine-do)| | |
| |[ OutputGainDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#outputgaindecibels-plasma)| | |
| |[ Ratio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#ratio-plasma-engine-docume)| | |
| |[ ReleaseMillisec](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#releasemillisec-plasma-eng)| | |
| |[ ThresholdDecibels](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md#thresholddecibels-plasma-e)| | |


 #  Properties


---  
 #  AttackMillisec : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time for the compressor to ramp to full effect after the input reaches the threshold.
> ``` lang=cpp, name=Lightning
> var AttackMillisec : Real


---  
 #  InputGainDecibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment applied to the audio input, in decibels.
> ``` lang=cpp, name=Lightning
> var InputGainDecibels : Real


---  
 #  KneeWidth : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The knee width of the compressor, in decibels.
> ``` lang=cpp, name=Lightning
> var KneeWidth : Real


---  
 #  OutputGainDecibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume adjustment applied to the compressor output, in decibels.
> ``` lang=cpp, name=Lightning
> var OutputGainDecibels : Real


---  
 #  Ratio : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The ratio of the volume reduction applied by the compressor.
> ``` lang=cpp, name=Lightning
> var Ratio : Real


---  
 #  ReleaseMillisec : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The time for the compressor to ramp from full effect to off after the input drops below the threshold.
> ``` lang=cpp, name=Lightning
> var ReleaseMillisec : Real


---  
 #  ThresholdDecibels : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The threshold, in decibels, at which the volume of the input is affected by the compressor.
> ``` lang=cpp, name=Lightning
> var ThresholdDecibels : Real


---  
 #  Methods


---  
 

 
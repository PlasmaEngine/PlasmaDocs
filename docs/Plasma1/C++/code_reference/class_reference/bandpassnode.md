 `Sound`

(NOTE) Applies a band pass filter to audio generated by its input SoundNodes (removes low and high frequencies)

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ CentralFrequency](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/bandpassnode.md#centralfrequency-plasma-en)|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
| |[ QualityFactor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/bandpassnode.md#qualityfactor-plasma-engin)| | |


 #  Properties


---  
 #  CentralFrequency : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The center frequency of the band. Frequencies above and below this band will be attenuated.
> ``` lang=cpp, name=Lightning
> var CentralFrequency : Real


---  
 #  QualityFactor : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The Q number of the band pass filter: higher numbers make the band smaller, while smaller numbers make it wider. The default value is 0.669.
> ``` lang=cpp, name=Lightning
> var QualityFactor : Real


---  
 #  Methods


---  
 

 
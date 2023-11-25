 `ContentMeta`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FileLoadType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundbuilder.md#fileloadtype-plasma-engine)|[buildercomponent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buildercomponent.md)| |
| |[ MaxVolume](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundbuilder.md#maxvolume-plasma-engine-do)| | |
| |[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundbuilder.md#name-plasma-engine-documen)| | |
| |[ Normalize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundbuilder.md#normalize-plasma-engine-do)| | |


 #  Properties


---  
 #  FileLoadType : [AudioFileLoadType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#audiofileloadtype)

> If Streamed is selected, or if Auto is selected and the file is longer than one minute, the sound file will be streamed from disk at runtime instead of loaded into memory. Streaming files can't be played multiple times simultaneously and can't use loop tails.
> ``` lang=cpp, name=Lightning
> var FileLoadType : AudioFileLoadType


---  
 #  MaxVolume : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The volume of the sound will be altered so that the highest volume peak matches this value. All audio samples will be adjusted equally.
> ``` lang=cpp, name=Lightning
> var MaxVolume : Real


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Normalize : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If true, the audio will be normalized when loaded so that the highest volume peak matches the MaxVolume value.
> ``` lang=cpp, name=Lightning
> var Normalize : Boolean


---  
 #  Methods


---  
 

 
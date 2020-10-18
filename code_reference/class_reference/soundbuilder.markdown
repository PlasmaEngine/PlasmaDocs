 `ContentMeta`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FileLoadType](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/soundbuilder.markdown#fileloadtype-plasma-engine)|[buildercomponent](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/buildercomponent.markdown)| |
| |[ MaxVolume](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/soundbuilder.markdown#maxvolume-plasma-engine-do)| | |
| |[ Name](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/soundbuilder.markdown#name-plasma-engine-documen)| | |
| |[ Normalize](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/soundbuilder.markdown#normalize-plasma-engine-do)| | |


 #  Properties


---  
 #  FileLoadType : [AudioFileLoadType](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#audiofileloadtype)

> If Streamed is selected, or if Auto is selected and the file is longer than one minute, the sound file will be streamed from disk at runtime instead of loaded into memory. Streaming files can't be played multiple times simultaneously and can't use loop tails.
> ``` lang=cpp, name=Lightning
> var FileLoadType : AudioFileLoadType


---  
 #  MaxVolume : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The volume of the sound will be altered so that the highest volume peak matches this value. All audio samples will be adjusted equally.
> ``` lang=cpp, name=Lightning
> var MaxVolume : Real


---  
 #  Name : [string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Normalize : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If true, the audio will be normalized when loaded so that the highest volume peak matches the MaxVolume value.
> ``` lang=cpp, name=Lightning
> var Normalize : Boolean


---  
 #  Methods


---  
 

 
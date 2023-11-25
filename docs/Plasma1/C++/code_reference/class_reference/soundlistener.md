 `Component` `Sound`



(NOTE) Uses the object's position to "hear" all SoundEmitters in the SoundSpace.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md#soundlistener-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ AttenuationScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md#attenuationscale-plasma-en)| | |
| |[ SoundNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md#soundnode-plasma-engine-do)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If this property is set to false the SoundListener will not produce any sound. All audio in the SoundSpace will continue to be processed, so this is not the same as pausing the sounds.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AttenuationScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The scale multiplier applied to the attenuation of sounds heard by this listener. If a sound uses a SoundAttenuator StopDistance of 20, and this value is 1.5, the attenuation will stop at 30.
> ``` lang=cpp, name=Lightning
> var AttenuationScale : Real


---  
 #  SoundNode : [soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)

 `read-only`

> The SoundNode associated with this SoundListener.
> ``` lang=cpp, name=Lightning
> var SoundNode : SoundNode


---  
 #  Methods


---  
 #  SoundListener : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SoundListener()
> ``` 


---  
 

 
 `Component` `Engine`



(NOTE) Settings for how the frame rate of the engine should be controlled.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frameratesettings.markdown#frameratesettings-void)|[ FrameRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frameratesettings.markdown#framerate-plasma-engine-do)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
| |[ LimitFrameRate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frameratesettings.markdown#limitframerate-plasma-engi)| | |
| |[ VerticalSync](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/frameratesettings.markdown#verticalsync-plasma-engine)| | |


 #  Properties


---  
 #  FrameRate : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> How many frames per second the engine should be limited at.
> ``` lang=cpp, name=Lightning
> var FrameRate : Integer


---  
 #  LimitFrameRate : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If the engine should limit the frame rate.
> ``` lang=cpp, name=Lightning
> var LimitFrameRate : Boolean


---  
 #  VerticalSync : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If the frame rate should sync with the monitor's refresh rate, superseded by LimitFrameRate.
> ``` lang=cpp, name=Lightning
> var VerticalSync : Boolean


---  
 #  Methods


---  
 #  FrameRateSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FrameRateSettings()
> ``` 


---  
 

 
 `Component` `Engine`



(NOTE) Time space component controls time for a Space.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Step](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#step-void)|[ Dt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#dt-plasma-engine-documenta)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#timespace-void)|[ DtOrZero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#dtorplasma-plasma-engine-doc)| | |
|[ TogglePause](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#togglepause-void)|[ Frame](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#frame-plasma-engine-docume)| | |
| |[ GloballyPaused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#globallypaused-plasma-engi)| | |
| |[ MaxDt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#maxdt-plasma-engine-docume)| | |
| |[ MinDt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#mindt-plasma-engine-docume)| | |
| |[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#paused-plasma-engine-docum)| | |
| |[ RealDt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#realdt-plasma-engine-docum)| | |
| |[ RealTimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#realtimepassed-plasma-engi)| | |
| |[ StepCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#stepcount-plasma-engine-do)| | |
| |[ TimeMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#timemode-plasma-engine-doc)| | |
| |[ TimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#timepassed-plasma-engine-d)| | |
| |[ TimeScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/timespace.markdown#timescale-plasma-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Dt : Real


---  
 #  DtOrZero : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var DtOrZero : Real


---  
 #  Frame : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The current frame we are on (starts at 0 and counts up for every frame that is run) This value counts up regardless of if the space is paused.
> ``` lang=cpp, name=Lightning
> var Frame : Integer


---  
 #  GloballyPaused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var GloballyPaused : Boolean


---  
 #  MaxDt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The maximum amount of time we send when running in 'ActualFrametime' mode If this value is set too high and the user does anything to pause their system or the game (example grabbing the window) then a large frame time will be sent out and physics objects will jump very far (causing tunneling and random bounces)
> ``` lang=cpp, name=Lightning
> var MaxDt : Real


---  
 #  MinDt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The minimum amount of time we send when running in 'ActualFrametime' mode Ideally this is set to a very small non-plasma value to prevent any division by plasma errors.
> ``` lang=cpp, name=Lightning
> var MinDt : Real


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If the time space is paused then we cease sending out logic update events When paused, the Dt will remain at whatever it was (it will NOT be set to 0)
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  RealDt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var RealDt : Real


---  
 #  RealTimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var RealTimePassed : Real


---  
 #  StepCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Causes the engine to update multiple times before rendering a frame.
> ``` lang=cpp, name=Lightning
> var StepCount : Integer


---  
 #  TimeMode : [TimeMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#timemode)

> When set to fixed framerate the Dt/frame time will never change (it will send whatever the project frame-rate-limiter is set to) This means it is important to run with a frame-rate limiter of some kind otherwise the game will appear to run much faster/slower Note: For determinism, you should always run in FixedFrametime mode When set to actual framerate we will send out the real time that the engine is encountering (clamped by MinDt / MaxDt)
> ``` lang=cpp, name=Lightning
> var TimeMode : TimeMode


---  
 #  TimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var TimePassed : Real


---  
 #  TimeScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Scale the speed of time for interesting effects like bullet time or fast paced gameplay. TimeScale is clamped to be positive.
> ``` lang=cpp, name=Lightning
> var TimeScale : Real


---  
 #  Methods


---  
 #  Step : Void

> Allows the engine to be advance one frame forward. Useful for debugging one frame at a time.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Step()
> ``` 


---  
 #  TimeSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function TimeSpace()
> ``` 


---  
 #  TogglePause : Void

> Toggles the state of paused.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function TogglePause()
> ``` 


---  
 

 
 `Engine`

(NOTE) Game pad is a object for getting game pad input.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonHeld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#isbuttonheld-plasma-engine)|[ GamepadIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#gamepadindex-plasma-engine)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ IsButtonPressed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#isbuttonpressed-plasma-eng)|[ IsActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#isactive-plasma-engine-doc)| | |
|[ IsButtonReleased](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#isbuttonreleased-plasma-en)|[ LeftStick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#leftstick-plasma-engine-do)| | |
|[ TimeButtonHeld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#timebuttonheld-plasma-engi)|[ LeftStickDelta](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#leftstickdelta-plasma-engi)| | |
|[ Vibrate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#vibrate-void)|[ LeftTrigger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#lefttrigger-plasma-engine)| | |
| |[ RightStick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#rightstick-plasma-engine-d)| | |
| |[ RightStickDelta](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#rightstickdelta-plasma-eng)| | |
| |[ RightTrigger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md#righttrigger-plasma-engine)| | |


 #  Properties


---  
 #  GamepadIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Index of this gamepad.
> ``` lang=cpp, name=Lightning
> var GamepadIndex : Integer


---  
 #  IsActive : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is this controller turned on and plugged in.
> ``` lang=cpp, name=Lightning
> var IsActive : Boolean


---  
 #  LeftStick : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Current offset [-1,1] from the center of the left stick.
> ``` lang=cpp, name=Lightning
> var LeftStick : Real2


---  
 #  LeftStickDelta : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Change in the left stick this frame.
> ``` lang=cpp, name=Lightning
> var LeftStickDelta : Real2


---  
 #  LeftTrigger : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Value of how much the Left Trigger is down. Range [0,1].
> ``` lang=cpp, name=Lightning
> var LeftTrigger : Real


---  
 #  RightStick : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Current offset [-1,1] from the center of the right stick.
> ``` lang=cpp, name=Lightning
> var RightStick : Real2


---  
 #  RightStickDelta : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Change in the right stick this frame.
> ``` lang=cpp, name=Lightning
> var RightStickDelta : Real2


---  
 #  RightTrigger : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Value of how much the Right Trigger is down. Range [0,1].
> ``` lang=cpp, name=Lightning
> var RightTrigger : Real


---  
 #  Methods


---  
 #  IsButtonHeld : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the button currently being held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IsButtonHeld(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonPressed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Has the button just been pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IsButtonPressed(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonReleased : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the button just been released.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IsButtonReleased(index : Integer) : Boolean
> ``` 


---  
 #  TimeButtonHeld : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How long has this button been held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function TimeButtonHeld(index : Integer) : Real
> ``` 


---  
 #  Vibrate : Void

> Vibrate this controller for a given time. Speed is a value between plasma and one.
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |LeftSpeed|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |RightSpeed|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function Vibrate(time : Real, LeftSpeed : Real, RightSpeed : Real)
> ``` 


---  
 

 
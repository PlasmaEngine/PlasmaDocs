 `Engine`

(NOTE) Game pad is a object for getting game pad input.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonHeld](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#isbuttonheld-plasma-engine)|[ GamepadIndex](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#gamepadindex-plasma-engine)|[eventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventobject.markdown)| |
|[ IsButtonPressed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#isbuttonpressed-plasma-eng)|[ IsActive](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#isactive-plasma-engine-doc)| | |
|[ IsButtonReleased](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#isbuttonreleased-plasma-en)|[ LeftStick](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#leftstick-plasma-engine-do)| | |
|[ TimeButtonHeld](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#timebuttonheld-plasma-engi)|[ LeftStickDelta](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#leftstickdelta-plasma-engi)| | |
|[ Vibrate](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#vibrate-void)|[ LeftTrigger](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#lefttrigger-plasma-engine)| | |
| |[ RightStick](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#rightstick-plasma-engine-d)| | |
| |[ RightStickDelta](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#rightstickdelta-plasma-eng)| | |
| |[ RightTrigger](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamepad.markdown#righttrigger-plasma-engine)| | |


 #  Properties


---  
 #  GamepadIndex : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Index of this gamepad.
> ``` lang=cpp, name=Lightning
> var GamepadIndex : Integer


---  
 #  IsActive : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is this controller turned on and plugged in.
> ``` lang=cpp, name=Lightning
> var IsActive : Boolean


---  
 #  LeftStick : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Current offset [-1,1] from the center of the left stick.
> ``` lang=cpp, name=Lightning
> var LeftStick : Real2


---  
 #  LeftStickDelta : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Change in the left stick this frame.
> ``` lang=cpp, name=Lightning
> var LeftStickDelta : Real2


---  
 #  LeftTrigger : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Value of how much the Left Trigger is down. Range [0,1].
> ``` lang=cpp, name=Lightning
> var LeftTrigger : Real


---  
 #  RightStick : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Current offset [-1,1] from the center of the right stick.
> ``` lang=cpp, name=Lightning
> var RightStick : Real2


---  
 #  RightStickDelta : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Change in the right stick this frame.
> ``` lang=cpp, name=Lightning
> var RightStickDelta : Real2


---  
 #  RightTrigger : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Value of how much the Right Trigger is down. Range [0,1].
> ``` lang=cpp, name=Lightning
> var RightTrigger : Real


---  
 #  Methods


---  
 #  IsButtonHeld : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is the button currently being held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsButtonHeld(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonPressed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Has the button just been pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsButtonPressed(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonReleased : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is the button just been released.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsButtonReleased(index : Integer) : Boolean
> ``` 


---  
 #  TimeButtonHeld : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> How long has this button been held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function TimeButtonHeld(index : Integer) : Real
> ``` 


---  
 #  Vibrate : Void

> Vibrate this controller for a given time. Speed is a value between plasma and one.
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |LeftSpeed|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |RightSpeed|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Vibrate(time : Real, LeftSpeed : Real, RightSpeed : Real)
> ``` 


---  
 

 
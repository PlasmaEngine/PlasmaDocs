 `Engine`

(NOTE) Gamepads is a collection of gamepads.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetGamePad](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.md#getgamepad-plasma-engine-d)|[ MaxGamepadCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.md#maxgamepadcount-plasma-eng)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ PauseVibration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.md#pausevibration-void)| | | |
|[ ResumeVibration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.md#resumevibration-void)| | | |


 #  Properties


---  
 #  MaxGamepadCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Gets the maximum number of supported gamepads.
> ``` lang=cpp, name=Lightning
> var MaxGamepadCount : Integer


---  
 #  Methods


---  
 #  GetGamePad : [gamepad](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.md)

> Get the gamepad for a given index from [0, GamepadCount].
> |Name|Type|Description|
> |---|---|---|
> |gamepadIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetGamePad(gamepadIndex : Integer) : Gamepad
> ``` 


---  
 #  PauseVibration : Void

> Pause Vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PauseVibration()
> ``` 


---  
 #  ResumeVibration : Void

> Resume vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ResumeVibration()
> ``` 


---  
 

 
 `Event` `Engine`



(NOTE) Gamepad events are send when a game pad button state is changed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Button](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepadevent.markdown#button-plasma-engine-docum)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ FlickDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepadevent.markdown#flickdirection-plasma-engi)| | |
| |[ FlickedStick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepadevent.markdown#flickedstick-plasma-engine)| | |
| |[ Gamepad](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepadevent.markdown#gamepad-plasma-engine-docu)| | |


 #  Properties


---  
 #  Button : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Button that was just pressed down or released up.
> ``` lang=cpp, name=Lightning
> var Button : Integer


---  
 #  FlickDirection : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

> The direction of the stick that was flicked (normalized)
> ``` lang=cpp, name=Lightning
> var FlickDirection : Real2


---  
 #  FlickedStick : [FlickedStick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#flickedstick)

> When responding to the 'GamepadStickFlicked' event, this will be set to the stick that was flicked.
> ``` lang=cpp, name=Lightning
> var FlickedStick : FlickedStick


---  
 #  Gamepad : [gamepad](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepad.markdown)

> Gamepad that generated this event.
> ``` lang=cpp, name=Lightning
> var Gamepad : Gamepad


---  
 #  Methods


---  
 

 
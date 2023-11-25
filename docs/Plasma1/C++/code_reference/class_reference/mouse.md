 `Engine`

(NOTE) Mouse object for Display System.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#isbuttondown-plasma-engine)|[ ClientPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#clientposition-plasma-engi)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ ToggleTrapped](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#toggletrapped-void)|[ Cursor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#cursor-plasma-engine-docum)| | |
| |[ CursorMovement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#cursormovement-plasma-engi)| | |
| |[ RawMovement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#rawmovement-plasma-engine)| | |
| |[ Trapped](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#trapped-plasma-engine-docu)| | |


 #  Properties


---  
 #  ClientPosition : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

 `read-only`

> The position of the mouse cursor relative to the application's top-left corner in pixels.
> ``` lang=cpp, name=Lightning
> var ClientPosition : Real2


---  
 #  Cursor : [Cursor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cursor)

> Set the cursor of the mouse.
> ``` lang=cpp, name=Lightning
> var Cursor : Cursor


---  
 #  CursorMovement : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

 `read-only`

> The movement of the mouse in pixels.
> ``` lang=cpp, name=Lightning
> var CursorMovement : Real2


---  
 #  RawMovement : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> High precision raw movement of the mouse.
> ``` lang=cpp, name=Lightning
> var RawMovement : Real2


---  
 #  Trapped : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Trap the mouse preventing it from moving.
> ``` lang=cpp, name=Lightning
> var Trapped : Boolean


---  
 #  Methods


---  
 #  IsButtonDown : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is a mouse button currently down?
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#mousebuttons)| |
> ``` lang=cpp, name=Lightning
> function IsButtonDown(button : MouseButtons) : Boolean
> ``` 


---  
 #  ToggleTrapped : Void

> Toggles if the mouse is currently trapped.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ToggleTrapped()
> ``` 


---  
 

 
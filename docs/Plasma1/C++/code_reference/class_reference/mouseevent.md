 `Event` `Widget`



(NOTE) Mouse events for actions concerning the mouse.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#isbuttonup-plasma-engine-d)|[ AltPressed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#altpressed-plasma-engine-d)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)|[mousedragevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousedragevent.md)|
| |[ Button](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#button-plasma-engine-docum)| |[mousefiledropevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousefiledropevent.md)|
| |[ ButtonDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#buttondown-plasma-engine-d)| |[viewportmouseevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md)|
| |[ CtrlPressed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#ctrlpressed-plasma-engine)| | |
| |[ HandledEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#handledevent-plasma-engine)| | |
| |[ Mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#mouse-plasma-engine-docume)| | |
| |[ Movement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#movement-plasma-engine-doc)| | |
| |[ Position](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#position-plasma-engine-doc)| | |
| |[ Scroll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#scroll-plasma-engine-docum)| | |
| |[ ShiftPressed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md#shiftpressed-plasma-engine)| | |


 #  Properties


---  
 #  AltPressed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var AltPressed : Boolean


---  
 #  Button : [MouseButtons](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#mousebuttons)

> 
> ``` lang=cpp, name=Lightning
> var Button : MouseButtons


---  
 #  ButtonDown : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> State of all the mouse buttons.
> ``` lang=cpp, name=Lightning
> var ButtonDown : Boolean


---  
 #  CtrlPressed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var CtrlPressed : Boolean


---  
 #  HandledEvent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var HandledEvent : Boolean


---  
 #  Mouse : [mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Mouse : Mouse


---  
 #  Movement : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> 
> ``` lang=cpp, name=Lightning
> var Movement : Real2


---  
 #  Position : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> 
> ``` lang=cpp, name=Lightning
> var Position : Real2


---  
 #  Scroll : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> 
> ``` lang=cpp, name=Lightning
> var Scroll : Real2


---  
 #  ShiftPressed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var ShiftPressed : Boolean


---  
 #  Methods


---  
 #  IsButtonUp : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#mousebuttons)| |
> ``` lang=cpp, name=Lightning
> function IsButtonUp(button : MouseButtons) : Boolean
> ``` 


---  
 

 
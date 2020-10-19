 `Event` `Widget`



(NOTE) Mouse events for actions concerning the mouse.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#isbuttonup-plasma-engine-d)|[ AltPressed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#altpressed-plasma-engine-d)|[event](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)|[mousedragevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousedragevent.markdown)|
| |[ Button](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#button-plasma-engine-docum)| |[mousefiledropevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousefiledropevent.markdown)|
| |[ ButtonDown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#buttondown-plasma-engine-d)| |[viewportmouseevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/viewportmouseevent.markdown)|
| |[ CtrlPressed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#ctrlpressed-plasma-engine)| | |
| |[ HandledEvent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#handledevent-plasma-engine)| | |
| |[ Mouse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#mouse-plasma-engine-docume)| | |
| |[ Movement](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#movement-plasma-engine-doc)| | |
| |[ Position](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#position-plasma-engine-doc)| | |
| |[ Scroll](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#scroll-plasma-engine-docum)| | |
| |[ ShiftPressed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouseevent.markdown#shiftpressed-plasma-engine)| | |


 #  Properties


---  
 #  AltPressed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var AltPressed : Boolean


---  
 #  Button : [MouseButtons](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#mousebuttons)

> 
> ``` lang=cpp, name=Lightning
> var Button : MouseButtons


---  
 #  ButtonDown : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> State of all the mouse buttons.
> ``` lang=cpp, name=Lightning
> var ButtonDown : Boolean


---  
 #  CtrlPressed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var CtrlPressed : Boolean


---  
 #  HandledEvent : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HandledEvent : Boolean


---  
 #  Mouse : [mouse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mouse.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Mouse : Mouse


---  
 #  Movement : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Movement : Real2


---  
 #  Position : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Position : Real2


---  
 #  Scroll : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Scroll : Real2


---  
 #  ShiftPressed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ShiftPressed : Boolean


---  
 #  Methods


---  
 #  IsButtonUp : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#mousebuttons)| |
> ``` lang=cpp, name=Lightning
> function IsButtonUp(button : MouseButtons) : Boolean
> ``` 


---  
 

 
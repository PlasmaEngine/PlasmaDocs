 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClientToScreen](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#clienttoscreen-plasma-engi)|[ ClientSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#clientsize-plasma-engine-d)|[threadsafeid32eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/threadsafeid32eventobject.md)|[windowsoswindow](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windowsoswindow.md)|
|[ HasFocus](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#hasfocus-plasma-engine-doc)|[ MinSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#minsize-plasma-engine-docu)| | |
|[ ScreenToClient](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#screentoclient-plasma-engi)|[ MouseCapture](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#mousecapture-plasma-engine)| | |
| |[ MouseCursor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#mousecursor-plasma-engine)| | |
| |[ MouseTrap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#mousetrap-plasma-engine-do)| | |
| |[ Parent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#parent-plasma-engine-docum)| | |
| |[ Position](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#position-plasma-engine-doc)| | |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#size-plasma-engine-documen)| | |
| |[ State](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#state-plasma-engine-docume)| | |
| |[ Title](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#title-plasma-engine-docume)| | |
| |[ Visible](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md#visible-plasma-engine-docu)| | |


 #  Properties


---  
 #  ClientSize : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> ``` lang=cpp, name=Lightning
> var ClientSize : Integer2


---  
 #  MinSize : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> ``` lang=cpp, name=Lightning
> var MinSize : Integer2


---  
 #  MouseCapture : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var MouseCapture : Boolean


---  
 #  MouseCursor : [Cursor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#cursor)

> 
> ``` lang=cpp, name=Lightning
> var MouseCursor : Cursor


---  
 #  MouseTrap : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var MouseTrap : Boolean


---  
 #  Parent : [oswindow](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/oswindow.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Parent : OsWindow


---  
 #  Position : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> ``` lang=cpp, name=Lightning
> var Position : Integer2


---  
 #  Size : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> ``` lang=cpp, name=Lightning
> var Size : Integer2


---  
 #  State : [WindowState](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#windowstate)

> 
> ``` lang=cpp, name=Lightning
> var State : WindowState


---  
 #  Title : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var Title : String


---  
 #  Visible : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var Visible : Boolean


---  
 #  Methods


---  
 #  ClientToScreen : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)| |
> ``` lang=cpp, name=Lightning
> function ClientToScreen(p0 : Integer2) : Integer2
> ``` 


---  
 #  HasFocus : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function HasFocus() : Boolean
> ``` 


---  
 #  ScreenToClient : [integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer2.md)| |
> ``` lang=cpp, name=Lightning
> function ScreenToClient(p0 : Integer2) : Integer2
> ``` 


---  
 

 
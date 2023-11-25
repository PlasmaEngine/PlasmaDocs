 `Gameplay`

(NOTE) Global functionality exposed to Lightning script. Bound as "Plasma" to script (e.g. Plasma.Keyboard) PlasmaStatic was used to avoid the conflict with namespace Plasma).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#connect-void)|[ Audio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#audio-plasma-engine-docume)| | |
|[ Disconnect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#disconnect-void)|[ Editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#editor-plasma-engine-docum)| | |
|[ DisconnectAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#disconnectall-void)|[ Engine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#engine-plasma-engine-docum)| | |
| |[ Environment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#environment-plasma-engine)| | |
| |[ Gamepads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#gamepads-plasma-engine-doc)| | |
| |[ Joysticks](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#joysticks-plasma-engine-do)| | |
| |[ Keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#keyboard-plasma-engine-doc)| | |
| |[ Mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#mouse-plasma-engine-docume)| | |
| |[ ObjectStore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#objectstore-plasma-engine)| | |
| |[ OsShell](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#osshell-plasma-engine-docu)| | |
| |[ ResourceSystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.md#resourcesystem-plasma-engi)| | |


 #  Properties


---  
 #  Audio : [audio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audio.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Audio : Audio


---  
 #  Editor : [editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/editor.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Editor : Editor


---  
 #  Engine : [engine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Engine : Engine


---  
 #  Environment : [environment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/environment.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Environment : Environment


---  
 #  Gamepads : [gamepads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Gamepads : Gamepads


---  
 #  Joysticks : [joysticks](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joysticks.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Joysticks : Joysticks


---  
 #  Keyboard : [keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Keyboard : Keyboard


---  
 #  Mouse : [mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Mouse : Mouse


---  
 #  ObjectStore : [objectstore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var ObjectStore : ObjectStore


---  
 #  OsShell : [osshell](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/osshell.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var OsShell : OsShell


---  
 #  ResourceSystem : [resourcesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcesystem.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var ResourceSystem : ResourceSystem


---  
 #  Methods


---  
 #  Connect : Void

 `static`

> Connection invokes the given delegate when sender dispatches the specified event.
> |Name|Type|Description|
> |---|---|---|
> |sender|Object| |
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |receiverDelegate|delegate()| |
> ``` lang=cpp, name=Lightning
> function Connect(sender : Object, eventId : String, receiverDelegate : delegate())
> ``` 


---  
 #  Disconnect : Void

 `static`

> Removes specified event connection, if connection delegate was a component method then receiver object is just the component.
> |Name|Type|Description|
> |---|---|---|
> |sender|Object| |
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |receiver|Object| |
> ``` lang=cpp, name=Lightning
> function Disconnect(sender : Object, eventId : String, receiver : Object)
> ``` 


---  
 #  DisconnectAll : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ||Object| |
> ||Object| |
> ``` lang=cpp, name=Lightning
> function DisconnectAll( : Object,  : Object)
> ``` 


---  
 

 
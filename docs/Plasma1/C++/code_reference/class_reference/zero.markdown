 `Gameplay`

(NOTE) Global functionality exposed to Lightning script. Bound as "Plasma" to script (e.g. Plasma.Keyboard) PlasmaStatic was used to avoid the conflict with namespace Plasma).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#connect-void)|[ Audio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#audio-plasma-engine-docume)| | |
|[ Disconnect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#disconnect-void)|[ Editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#editor-plasma-engine-docum)| | |
|[ DisconnectAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#disconnectall-void)|[ Engine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#engine-plasma-engine-docum)| | |
| |[ Environment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#environment-plasma-engine)| | |
| |[ Gamepads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#gamepads-plasma-engine-doc)| | |
| |[ Joysticks](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#joysticks-plasma-engine-do)| | |
| |[ Keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#keyboard-plasma-engine-doc)| | |
| |[ Mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#mouse-plasma-engine-docume)| | |
| |[ ObjectStore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#objectstore-plasma-engine)| | |
| |[ OsShell](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#osshell-plasma-engine-docu)| | |
| |[ ResourceSystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown#resourcesystem-plasma-engi)| | |


 #  Properties


---  
 #  Audio : [audio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/audio.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Audio : Audio


---  
 #  Editor : [editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/editor.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Editor : Editor


---  
 #  Engine : [engine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Engine : Engine


---  
 #  Environment : [environment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/environment.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Environment : Environment


---  
 #  Gamepads : [gamepads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamepads.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Gamepads : Gamepads


---  
 #  Joysticks : [joysticks](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joysticks.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Joysticks : Joysticks


---  
 #  Keyboard : [keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Keyboard : Keyboard


---  
 #  Mouse : [mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Mouse : Mouse


---  
 #  ObjectStore : [objectstore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectstore.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var ObjectStore : ObjectStore


---  
 #  OsShell : [osshell](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/osshell.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var OsShell : OsShell


---  
 #  ResourceSystem : [resourcesystem](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/resourcesystem.markdown)

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
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
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
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
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
 

 
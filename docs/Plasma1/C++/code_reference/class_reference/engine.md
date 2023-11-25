 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CrashEngine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#crashengine-void)|[ GameSessions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#gamesessions-plasma-engine)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ CreateGameSession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#creategamesession-plasma-e)| | | |
|[ CreateGameSessionFromArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#creategamesessionfromarc)| | | |
|[ DebugBreak](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#debugbreak-void)| | | |
|[ GetCurrentInputDevice](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#getcurrentinputdevice-ze)| | | |
|[ RebuildArchetypes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#rebuildarchetypes-void)| | | |
|[ Terminate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.md#terminate-void)| | | |


 #  Properties


---  
 #  GameSessions : [gamesessionrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesessionrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var GameSessions : GameSessionRange


---  
 #  Methods


---  
 #  CrashEngine : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CrashEngine()
> ``` 


---  
 #  CreateGameSession : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateGameSession() : GameSession
> ``` 


---  
 #  CreateGameSessionFromArchetype : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function CreateGameSessionFromArchetype(p0 : Archetype) : GameSession
> ``` 


---  
 #  DebugBreak : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugBreak()
> ``` 


---  
 #  GetCurrentInputDevice : [InputDevice](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#inputdevice)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetCurrentInputDevice() : InputDevice
> ``` 


---  
 #  RebuildArchetypes : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function RebuildArchetypes(p0 : Archetype)
> ``` 


---  
 #  Terminate : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Terminate()
> ``` 


---  
 

 
 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CrashEngine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#crashengine-void)|[ GameSessions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#gamesessions-plasma-engine)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.markdown)| |
|[ CreateGameSession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#creategamesession-plasma-e)| | | |
|[ CreateGameSessionFromArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#creategamesessionfromarc)| | | |
|[ DebugBreak](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#debugbreak-void)| | | |
|[ GetCurrentInputDevice](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#getcurrentinputdevice-ze)| | | |
|[ RebuildArchetypes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#rebuildarchetypes-void)| | | |
|[ Terminate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/engine.markdown#terminate-void)| | | |


 #  Properties


---  
 #  GameSessions : [gamesessionrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesessionrange.markdown)

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
 #  CreateGameSession : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateGameSession() : GameSession
> ``` 


---  
 #  CreateGameSessionFromArchetype : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.markdown)| |
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
 #  GetCurrentInputDevice : [InputDevice](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#inputdevice)

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
> |p0|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.markdown)| |
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
 

 
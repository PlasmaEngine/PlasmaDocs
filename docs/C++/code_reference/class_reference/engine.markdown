 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CrashEngine](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#crashengine-void)|[ GameSessions](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#gamesessions-plasma-engine)|[eventobject](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/eventobject.markdown)| |
|[ CreateGameSession](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#creategamesession-plasma-e)| | | |
|[ CreateGameSessionFromArchetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#creategamesessionfromarc)| | | |
|[ DebugBreak](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#debugbreak-void)| | | |
|[ GetCurrentInputDevice](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#getcurrentinputdevice-ze)| | | |
|[ RebuildArchetypes](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#rebuildarchetypes-void)| | | |
|[ Terminate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/engine.markdown#terminate-void)| | | |


 #  Properties


---  
 #  GameSessions : [gamesessionrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gamesessionrange.markdown)

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
 #  CreateGameSession : [gamesession](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gamesession.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateGameSession() : GameSession
> ``` 


---  
 #  CreateGameSessionFromArchetype : [gamesession](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gamesession.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
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
 #  GetCurrentInputDevice : [InputDevice](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#inputdevice)

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
> |p0|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/archetype.markdown)| |
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
 

 
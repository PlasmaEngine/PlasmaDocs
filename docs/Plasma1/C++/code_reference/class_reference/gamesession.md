 `Engine`

(NOTE) The GameSession manages all spaces and data for a a game.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateNamedSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#createnamedspace-plasma-en)|[ AllSpaces](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#allspaces-plasma-engine-do)|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
|[ CreateSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#createspace-plasma-engine)|[ Focused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#focused-plasma-engine-docu)| | |
|[ FindAllSpacesByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#findallspacesbyname-plasma)|[ FullScreen](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#fullscreen-plasma-engine-d)| | |
|[ FindSpaceByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#findspacebyname-plasma-eng)|[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#paused-plasma-engine-docum)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#gamesession-void)|[ Resolution](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#resolution-plasma-engine-d)| | |
|[ IsEditorMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#iseditormode-plasma-engine)| | | |
|[ Pause](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#pause-void)| | | |
|[ Quit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#quit-void)| | | |
|[ RequestQuit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#requestquit-void)| | | |
|[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md#start-void)| | | |


 #  Properties


---  
 #  AllSpaces : [spacemapvaluerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spacemapvaluerange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllSpaces : SpaceMapValueRange


---  
 #  Focused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Focused : Boolean


---  
 #  FullScreen : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var FullScreen : Boolean


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls if the game session is paused which prevents updates to all spaces owned by this game.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Resolution : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Resolution : Real2


---  
 #  Methods


---  
 #  CreateNamedSpace : [space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)

> Create a space from an archetype with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function CreateNamedSpace(name : String, archetype : Archetype) : Space
> ``` 


---  
 #  CreateSpace : [space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)

> Create a space in the game. Use the archetype's name.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Lightning
> function CreateSpace(archetype : Archetype) : Space
> ``` 


---  
 #  FindAllSpacesByName : [spacemapvaluerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spacemapvaluerange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindAllSpacesByName(name : String) : SpaceMapValueRange
> ``` 


---  
 #  FindSpaceByName : [space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)

> Find a named space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindSpaceByName(name : String) : Space
> ``` 


---  
 #  GameSession : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GameSession()
> ``` 


---  
 #  IsEditorMode : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsEditorMode() : Boolean
> ``` 


---  
 #  Pause : Void

> Pauses the game session which prevents updates to all spaces owned by this game.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Pause()
> ``` 


---  
 #  Quit : Void

> Quit the game and exit the engine if not in editor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Quit()
> ``` 


---  
 #  RequestQuit : Void

> Request to quit sending out the GameRequestQuit event.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RequestQuit()
> ``` 


---  
 #  Start : Void

> Start the game.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Start()
> ``` 


---  
 

 
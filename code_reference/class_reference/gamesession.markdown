 `Engine`

(NOTE) The GameSession manages all spaces and data for a a game.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateNamedSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#createnamedspace-plasma-en)|[ AllSpaces](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#allspaces-plasma-engine-do)|[cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)| |
|[ CreateSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#createspace-plasma-engine)|[ Focused](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#focused-plasma-engine-docu)| | |
|[ FindAllSpacesByName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#findallspacesbyname-plasma)|[ FullScreen](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#fullscreen-plasma-engine-d)| | |
|[ FindSpaceByName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#findspacebyname-plasma-eng)|[ Paused](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#paused-plasma-engine-docum)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#gamesession-void)|[ Resolution](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#resolution-plasma-engine-d)| | |
|[ IsEditorMode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#iseditormode-plasma-engine)| | | |
|[ Pause](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#pause-void)| | | |
|[ Quit](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#quit-void)| | | |
|[ RequestQuit](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#requestquit-void)| | | |
|[ Start](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/gamesession.markdown#start-void)| | | |


 #  Properties


---  
 #  AllSpaces : [spacemapvaluerange](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/spacemapvaluerange.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AllSpaces : SpaceMapValueRange


---  
 #  Focused : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Focused : Boolean


---  
 #  FullScreen : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var FullScreen : Boolean


---  
 #  Paused : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls if the game session is paused which prevents updates to all spaces owned by this game.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Resolution : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Resolution : Real2


---  
 #  Methods


---  
 #  CreateNamedSpace : [space](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/space.markdown)

> Create a space from an archetype with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |archetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/archetype.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateNamedSpace(name : String, archetype : Archetype) : Space
> ``` 


---  
 #  CreateSpace : [space](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/space.markdown)

> Create a space in the game. Use the archetype's name.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/archetype.markdown)| |
> ``` lang=cpp, name=Lightning
> function CreateSpace(archetype : Archetype) : Space
> ``` 


---  
 #  FindAllSpacesByName : [spacemapvaluerange](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/spacemapvaluerange.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function FindAllSpacesByName(name : String) : SpaceMapValueRange
> ``` 


---  
 #  FindSpaceByName : [space](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/space.markdown)

> Find a named space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
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
 #  IsEditorMode : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

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
 

 
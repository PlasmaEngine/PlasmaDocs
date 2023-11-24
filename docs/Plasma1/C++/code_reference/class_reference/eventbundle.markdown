 `Networking`

(NOTE) Event Bundle. Serialized event storage container.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#addevent-plasma-engine-doc)|[ GameSession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#gamesession-plasma-engine)|Object| |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#clear-void)|[ IsEmpty](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#isempty-plasma-engine-docu)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#eventbundle-void)| | | |
|[ GetEvents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#getevents-plasma-engine-do)| | | |
|[ RemoveEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown#removeevent-plasma-engine)| | | |


 #  Properties


---  
 #  GameSession : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.markdown)

> Returns the game session.
> ``` lang=cpp, name=Lightning
> var GameSession : GameSession


---  
 #  IsEmpty : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the event bundle is empty (doesn't contain any events), else false.
> ``` lang=cpp, name=Lightning
> var IsEmpty : Boolean


---  
 #  Methods


---  
 #  AddEvent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Adds the event to back of the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddEvent(event : Event) : Boolean
> ``` 


---  
 #  Clear : Void

> Clears the event bundle.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function EventBundle()
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function EventBundle(event : Event)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |rhs|[eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)| |
> ``` lang=cpp, name=Lightning
> function EventBundle(rhs : EventBundle)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |gameSession|[gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.markdown)| |
> ``` lang=cpp, name=Lightning
> function EventBundle(gameSession : GameSession)
> ``` 


---  
 #  EventBundle : Void

 `constructor`

> Constructors.
> |Name|Type|Description|
> |---|---|---|
> |gameSession|[gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.markdown)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function EventBundle(gameSession : GameSession, event : Event)
> ``` 


---  
 #  GetEvents : [eventrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventrange.markdown)

> Returns all the events that have been added to the event bundle.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetEvents() : EventRange
> ``` 


---  
 #  RemoveEvent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Removes the event specified from the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveEvent(event : Event) : Boolean
> ``` 


---  
 #  RemoveEvent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Removes the event specified from the event bundle. Returns true if successful, else false (an event of that type has already been added).
> |Name|Type|Description|
> |---|---|---|
> ||[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveEvent( : String) : Boolean
> ``` 


---  
 

 
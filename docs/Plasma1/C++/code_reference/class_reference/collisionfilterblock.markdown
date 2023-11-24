 `Physics`

(NOTE) Used to specify which collision group events should be sent out for a CollisionFilter. Allows customizing who gets events (in the filter pair) and what event name is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BlockType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilterblock.markdown#blocktype-plasma-engine-do)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.markdown)|[collisionendblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionendblock.markdown)|
| |[ EventOverride](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilterblock.markdown#eventoverride-plasma-engin)| |[collisionpersistedblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionpersistedblock.markdown)|
| |[ SendEventsToA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilterblock.markdown#sendeventstoa-plasma-engin)| |[collisionstartblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionstartblock.markdown)|
| |[ SendEventsToB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilterblock.markdown#sendeventstob-plasma-engin)| |[presolveblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/presolveblock.markdown)|
| |[ SendEventsToSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisionfilterblock.markdown#sendeventstospace-plasma-e)| | |


 #  Properties


---  
 #  BlockType : [CollisionFilterBlockType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#collisionfilterblocktype)

 `read-only`

> What type of collision filter block is this?
> ``` lang=cpp, name=Lightning
> var BlockType : CollisionFilterBlockType


---  
 #  EventOverride : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> What event name to send out when this block triggers. If left empty the default name will be used (e.g. GroupCollisionStarted).
> ``` lang=cpp, name=Lightning
> var EventOverride : String


---  
 #  SendEventsToA : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Does the first object in the filter get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToA : Boolean


---  
 #  SendEventsToB : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Does the second object in the filter get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToB : Boolean


---  
 #  SendEventsToSpace : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Does the active space of the objects get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToSpace : Boolean


---  
 #  Methods


---  
 

 
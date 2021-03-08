 `Physics`

(NOTE) Used to specify which collision group events should be sent out for a CollisionFilter. Allows customizing who gets events (in the filter pair) and what event name is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BlockType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown#blocktype-plasma-engine-do)|[safeid32object](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/safeid32object.markdown)|[collisionendblock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionendblock.markdown)|
| |[ EventOverride](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown#eventoverride-plasma-engin)| |[collisionpersistedblock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionpersistedblock.markdown)|
| |[ SendEventsToA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown#sendeventstoa-plasma-engin)| |[collisionstartblock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionstartblock.markdown)|
| |[ SendEventsToB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown#sendeventstob-plasma-engin)| |[presolveblock](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/presolveblock.markdown)|
| |[ SendEventsToSpace](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisionfilterblock.markdown#sendeventstospace-plasma-e)| | |


 #  Properties


---  
 #  BlockType : [CollisionFilterBlockType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#collisionfilterblocktype)

 `read-only`

> What type of collision filter block is this?
> ``` lang=cpp, name=Lightning
> var BlockType : CollisionFilterBlockType


---  
 #  EventOverride : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> What event name to send out when this block triggers. If left empty the default name will be used (e.g. GroupCollisionStarted).
> ``` lang=cpp, name=Lightning
> var EventOverride : String


---  
 #  SendEventsToA : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Does the first object in the filter get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToA : Boolean


---  
 #  SendEventsToB : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Does the second object in the filter get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToB : Boolean


---  
 #  SendEventsToSpace : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Does the active space of the objects get this event type sent to it?
> ``` lang=cpp, name=Lightning
> var SendEventsToSpace : Boolean


---  
 #  Methods


---  
 

 
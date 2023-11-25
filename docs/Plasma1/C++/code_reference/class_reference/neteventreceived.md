 `Event` `Networking`



(NOTE) Dispatched before a received net event is dispatched.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Destination](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/neteventreceived.md#destination-plasma-engine)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ NetEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/neteventreceived.md#netevent-plasma-engine-doc)| | |
| |[ ReturnAllow](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/neteventreceived.md#returnallow-plasma-engine)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/neteventreceived.md#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Destination : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> Dispatch destination object (null if the net object could not be found locally).
> ``` lang=cpp, name=Lightning
> var Destination : Cog


---  
 #  NetEvent : [event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)

 `read-only`

> Network event received.
> ``` lang=cpp, name=Lightning
> var NetEvent : Event


---  
 #  ReturnAllow : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Return: Allow the received network event to be dispatched on the destination object?
> ``` lang=cpp, name=Lightning
> var ReturnAllow : Boolean


---  
 #  TheirNetPeerId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
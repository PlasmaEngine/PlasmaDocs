 `Event` `Networking`



(NOTE) Dispatched before a received net event is dispatched.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Destination](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/neteventreceived.markdown#destination-plasma-engine)|[event](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/event.markdown)| |
| |[ NetEvent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/neteventreceived.markdown#netevent-plasma-engine-doc)| | |
| |[ ReturnAllow](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/neteventreceived.markdown#returnallow-plasma-engine)| | |
| |[ TheirNetPeerId](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/neteventreceived.markdown#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Destination : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

 `read-only`

> Dispatch destination object (null if the net object could not be found locally).
> ``` lang=cpp, name=Lightning
> var Destination : Cog


---  
 #  NetEvent : [event](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/event.markdown)

 `read-only`

> Network event received.
> ``` lang=cpp, name=Lightning
> var NetEvent : Event


---  
 #  ReturnAllow : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Return: Allow the received network event to be dispatched on the destination object?
> ``` lang=cpp, name=Lightning
> var ReturnAllow : Boolean


---  
 #  TheirNetPeerId : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
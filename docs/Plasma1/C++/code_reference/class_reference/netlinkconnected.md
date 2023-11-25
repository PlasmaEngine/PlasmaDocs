 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a connect confirmation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkconnected.md#direction-plasma-engine-do)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkconnected.md#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkconnected.md#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Lightning
> var Direction : TransmissionDirection


---  
 #  TheirIpAddress : [ipaddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
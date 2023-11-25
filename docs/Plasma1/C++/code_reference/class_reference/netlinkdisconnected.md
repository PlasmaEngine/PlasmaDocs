 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a disconnect notice. Their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkdisconnected.md#direction-plasma-engine-do)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ DisconnectReason](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkdisconnected.md#disconnectreason-plasma-en)| | |
| |[ RequestBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkdisconnected.md#requestbundle-plasma-engin)| | |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkdisconnected.md#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netlinkdisconnected.md#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Lightning
> var Direction : TransmissionDirection


---  
 #  DisconnectReason : [DisconnectReason](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#disconnectreason)

 `read-only`

> Disconnect reason.
> ``` lang=cpp, name=Lightning
> var DisconnectReason : DisconnectReason


---  
 #  RequestBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.md)

 `read-only`

> Bundled request event data.
> ``` lang=cpp, name=Lightning
> var RequestBundle : EventBundle


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
 

 
 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a disconnect notice. Their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkdisconnected.markdown#direction-plasma-engine-do)|[event](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/event.markdown)| |
| |[ DisconnectReason](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkdisconnected.markdown#disconnectreason-plasma-en)| | |
| |[ RequestBundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkdisconnected.markdown#requestbundle-plasma-engin)| | |
| |[ TheirIpAddress](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkdisconnected.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkdisconnected.markdown#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Lightning
> var Direction : TransmissionDirection


---  
 #  DisconnectReason : [DisconnectReason](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#disconnectreason)

 `read-only`

> Disconnect reason.
> ``` lang=cpp, name=Lightning
> var DisconnectReason : DisconnectReason


---  
 #  RequestBundle : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Bundled request event data.
> ``` lang=cpp, name=Lightning
> var RequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
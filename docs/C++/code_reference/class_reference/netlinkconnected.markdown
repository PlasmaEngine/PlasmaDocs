 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a connect confirmation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkconnected.markdown#direction-plasma-engine-do)|[event](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/event.markdown)| |
| |[ TheirIpAddress](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkconnected.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netlinkconnected.markdown#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Lightning
> var Direction : TransmissionDirection


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
 

 
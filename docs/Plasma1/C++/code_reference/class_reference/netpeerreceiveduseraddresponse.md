 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurNetUserId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#ournetuserid-plasma-engine)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ OurRequestBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#ourrequestbundle-plasma-en)| | |
| |[ TheirAddResponse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theiraddresponse-plasma-en)| | |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theirnetpeerid-plasma-engi)| | |
| |[ TheirResponseBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theirresponsebundle-plasma)| | |


 #  Properties


---  
 #  OurNetUserId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Our net user ID (set only if accepted).
> ``` lang=cpp, name=Lightning
> var OurNetUserId : Integer


---  
 #  OurRequestBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.md)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Lightning
> var OurRequestBundle : EventBundle


---  
 #  TheirAddResponse : [NetUserAddResponse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#netuseraddresponse)

 `read-only`

> Their add response.
> ``` lang=cpp, name=Lightning
> var TheirAddResponse : NetUserAddResponse


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
 #  TheirResponseBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.md)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Lightning
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
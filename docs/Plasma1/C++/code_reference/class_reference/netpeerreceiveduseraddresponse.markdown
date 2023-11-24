 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurNetUserId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#ournetuserid-plasma-engine)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ OurRequestBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#ourrequestbundle-plasma-en)| | |
| |[ TheirAddResponse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#theiraddresponse-plasma-en)| | |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#theirnetpeerid-plasma-engi)| | |
| |[ TheirResponseBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddresponse.markdown#theirresponsebundle-plasma)| | |


 #  Properties


---  
 #  OurNetUserId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Our net user ID (set only if accepted).
> ``` lang=cpp, name=Lightning
> var OurNetUserId : Integer


---  
 #  OurRequestBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Lightning
> var OurRequestBundle : EventBundle


---  
 #  TheirAddResponse : [NetUserAddResponse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#netuseraddresponse)

 `read-only`

> Their add response.
> ``` lang=cpp, name=Lightning
> var TheirAddResponse : NetUserAddResponse


---  
 #  TheirIpAddress : [ipaddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  TheirResponseBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Lightning
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
 `Event` `Networking`



(NOTE) Dispatched after sending a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurAddResponse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#ouraddresponse-plasma-engi)|[event](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/event.markdown)| |
| |[ OurResponseBundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#ourresponsebundle-plasma-e)| | |
| |[ TheirIpAddress](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#theirnetpeerid-plasma-engi)| | |
| |[ TheirNetUser](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#theirnetuser-plasma-engine)| | |
| |[ TheirNetUserId](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#theirnetuserid-plasma-engi)| | |
| |[ TheirRequestBundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/netpeersentuseraddresponse.markdown#theirrequestbundle-plasma)| | |


 #  Properties


---  
 #  OurAddResponse : [NetUserAddResponse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#netuseraddresponse)

 `read-only`

> Our add response.
> ``` lang=cpp, name=Lightning
> var OurAddResponse : NetUserAddResponse


---  
 #  OurResponseBundle : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled response event data.
> ``` lang=cpp, name=Lightning
> var OurResponseBundle : EventBundle


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
 #  TheirNetUser : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

 `read-only`

> Their net user object about to be added (set only if accepted).
> ``` lang=cpp, name=Lightning
> var TheirNetUser : Cog


---  
 #  TheirNetUserId : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net user ID (set only if accepted).
> ``` lang=cpp, name=Lightning
> var TheirNetUserId : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Lightning
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ReturnOurAddResponse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#returnouraddresponse-zer)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ ReturnOurResponseBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#returnourresponsebundle)| | |
| |[ ReturnTheirNetUser](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#returntheirnetuser-plasma)| | |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#theirnetpeerid-plasma-engi)| | |
| |[ TheirNetUserId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#theirnetuserid-plasma-engi)| | |
| |[ TheirRequestBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeerreceiveduseraddrequest.markdown#theirrequestbundle-plasma)| | |


 #  Properties


---  
 #  ReturnOurAddResponse : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Return: Our add response (accept the add request?).
> ``` lang=cpp, name=Lightning
> var ReturnOurAddResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)

> Return: Our bundled response event data.
> ``` lang=cpp, name=Lightning
> var ReturnOurResponseBundle : EventBundle


---  
 #  ReturnTheirNetUser : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> Return: Their network user object (must have a NetUser component).
> ``` lang=cpp, name=Lightning
> var ReturnTheirNetUser : Cog


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
 #  TheirNetUserId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net user ID (released back to the store if not accepted).
> ``` lang=cpp, name=Lightning
> var TheirNetUserId : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Lightning
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
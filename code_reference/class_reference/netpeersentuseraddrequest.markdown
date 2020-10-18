 `Event` `Networking`



(NOTE) Dispatched after sending a net user add request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurRequestBundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentuseraddrequest.markdown#ourrequestbundle-plasma-en)|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ TheirIpAddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentuseraddrequest.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentuseraddrequest.markdown#theirnetpeerid-plasma-engi)| | |


 #  Properties


---  
 #  OurRequestBundle : [eventbundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Lightning
> var OurRequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
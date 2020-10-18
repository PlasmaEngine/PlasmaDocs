 `Event` `Networking`



(NOTE) Dispatched after sending a connect response. If denied, their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurConnectResponse](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#ourconnectresponse-plasma)|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ OurIpAddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#ouripaddress-plasma-engine)| | |
| |[ OurResponseBundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#ourresponsebundle-plasma-e)| | |
| |[ TheirIpAddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirNetPeerId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#theirnetpeerid-plasma-engi)| | |
| |[ TheirPendingUserAddRequestCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#theirpendinguseraddreque)| | |
| |[ TheirRequestBundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.markdown#theirrequestbundle-plasma)| | |


 #  Properties


---  
 #  OurConnectResponse : [ConnectResponse](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#connectresponse)

 `read-only`

> Our connect response.
> ``` lang=cpp, name=Lightning
> var OurConnectResponse : ConnectResponse


---  
 #  OurIpAddress : [ipaddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Lightning
> var OurIpAddress : IpAddress


---  
 #  OurResponseBundle : [eventbundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled response event data.
> ``` lang=cpp, name=Lightning
> var OurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their net peer ID (set only if accepted).
> ``` lang=cpp, name=Lightning
> var TheirNetPeerId : Integer


---  
 #  TheirPendingUserAddRequestCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Lightning
> var TheirPendingUserAddRequestCount : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Lightning
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
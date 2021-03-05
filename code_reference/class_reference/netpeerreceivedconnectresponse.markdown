 `Event` `Networking`



(NOTE) Dispatched after receiving a connect response. If accepted, our net peer ID is set immediately before this and a connect confirmation is sent after this. If denied, our net peer ID is cleared and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurIpAddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#ouripaddress-plasma-engine)|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ OurNetPeerId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#ournetpeerid-plasma-engine)| | |
| |[ OurPendingUserAddRequestCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#ourpendinguseraddrequest)| | |
| |[ OurRequestBundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#ourrequestbundle-plasma-en)| | |
| |[ TheirConnectResponse](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#theirconnectresponse-zer)| | |
| |[ TheirIpAddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirResponseBundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectresponse.markdown#theirresponsebundle-plasma)| | |


 #  Properties


---  
 #  OurIpAddress : [ipaddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Lightning
> var OurIpAddress : IpAddress


---  
 #  OurNetPeerId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Our net peer ID (set only if accepted).
> ``` lang=cpp, name=Lightning
> var OurNetPeerId : Integer


---  
 #  OurPendingUserAddRequestCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Our pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Lightning
> var OurPendingUserAddRequestCount : Integer


---  
 #  OurRequestBundle : [eventbundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Lightning
> var OurRequestBundle : EventBundle


---  
 #  TheirConnectResponse : [ConnectResponse](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#connectresponse)

 `read-only`

> Their connect response.
> ``` lang=cpp, name=Lightning
> var TheirConnectResponse : ConnectResponse


---  
 #  TheirIpAddress : [ipaddress](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirResponseBundle : [eventbundle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Lightning
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
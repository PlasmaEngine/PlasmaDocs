 `Event` `Networking`



(NOTE) Dispatched after receiving a connect request. If accepted, their net peer ID is assigned immediately after this. Return true to accept the connect request, else false.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurIpAddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#ouripaddress-plasma-engine)|[event](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ ReturnOurConnectResponse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#returnourconnectresponse)| | |
| |[ ReturnOurResponseBundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#returnourresponsebundle)| | |
| |[ TheirIpAddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#theiripaddress-plasma-engi)| | |
| |[ TheirPendingUserAddRequestCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#theirpendinguseraddreque)| | |
| |[ TheirRequestBundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.markdown#theirrequestbundle-plasma)| | |


 #  Properties


---  
 #  OurIpAddress : [ipaddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Lightning
> var OurIpAddress : IpAddress


---  
 #  ReturnOurConnectResponse : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Return: Our connect response (accept the connect request?).
> ``` lang=cpp, name=Lightning
> var ReturnOurConnectResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

> Return: Our bundled response event data.
> ``` lang=cpp, name=Lightning
> var ReturnOurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  TheirPendingUserAddRequestCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Their pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Lightning
> var TheirPendingUserAddRequestCount : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Lightning
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
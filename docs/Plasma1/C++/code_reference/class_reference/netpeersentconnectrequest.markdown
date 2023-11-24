 `Event` `Networking`



(NOTE) Dispatched after sending a connect request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurPendingUserAddRequestCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeersentconnectrequest.markdown#ourpendinguseraddrequest)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ OurRequestBundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeersentconnectrequest.markdown#ourrequestbundle-plasma-en)| | |
| |[ TheirIpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeersentconnectrequest.markdown#theiripaddress-plasma-engi)| | |


 #  Properties


---  
 #  OurPendingUserAddRequestCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Our pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Lightning
> var OurPendingUserAddRequestCount : Integer


---  
 #  OurRequestBundle : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Lightning
> var OurRequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Lightning
> var TheirIpAddress : IpAddress


---  
 #  Methods


---  
 

 
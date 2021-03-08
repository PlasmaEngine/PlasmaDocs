 `Networking`

(NOTE) Describes a network host.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BasicHostInfo](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#basichostinfo-plasma-engin)|[safeid32](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/safeid32.markdown)| |
| |[ ExtraHostInfo](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#extrahostinfo-plasma-engin)| | |
| |[ IpAddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#ipaddress-plasma-engine-do)| | |
| |[ Latency](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#latency-plasma-engine-docu)| | |
| |[ Network](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#network-plasma-engine-docu)| | |
| |[ RoundTripTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown#roundtriptime-plasma-engin)| | |


 #  Properties


---  
 #  BasicHostInfo : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Basic host info (limited to 480 bytes).
> ``` lang=cpp, name=Lightning
> var BasicHostInfo : EventBundle


---  
 #  ExtraHostInfo : [eventbundle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventbundle.markdown)

 `read-only`

> Extra host info.
> ``` lang=cpp, name=Lightning
> var ExtraHostInfo : EventBundle


---  
 #  IpAddress : [ipaddress](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ipaddress.markdown)

 `read-only`

> Host's IP address.
> ``` lang=cpp, name=Lightning
> var IpAddress : IpAddress


---  
 #  Latency : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns the estimated latency ((RTT/2)) in milliseconds from our peer to this host.
> ``` lang=cpp, name=Lightning
> var Latency : Integer


---  
 #  Network : [Network](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#network)

 `read-only`

> Host's network residence.
> ``` lang=cpp, name=Lightning
> var Network : Network


---  
 #  RoundTripTime : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns the round-trip time (RTT) in milliseconds from our peer to this host.
> ``` lang=cpp, name=Lightning
> var RoundTripTime : Integer


---  
 #  Methods


---  
 

 
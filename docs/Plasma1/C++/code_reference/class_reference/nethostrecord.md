 `Networking`

(NOTE) NetHostRecord. A record that contains the basic information of a game server. After a certain lifetime records expire on the master server.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BasicHostInfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostrecord.md#basichostinfo-plasma-engin)|[safeid32](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32.md)| |
| |[ IpAddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostrecord.md#ipaddress-plasma-engine-do)| | |
| |[ Lifetime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostrecord.md#lifetime-plasma-engine-doc)| | |


 #  Properties


---  
 #  BasicHostInfo : [eventbundle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventbundle.md)

 `read-only`

> The info published along with their record. Contains game server specific data.
> ``` lang=cpp, name=Lightning
> var BasicHostInfo : EventBundle


---  
 #  IpAddress : [ipaddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md)

 `read-only`

> The IpAddress associated with this record. This is who published it.
> ``` lang=cpp, name=Lightning
> var IpAddress : IpAddress


---  
 #  Lifetime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> How long has this record been alive in seconds?
> ``` lang=cpp, name=Lightning
> var Lifetime : Real


---  
 #  Methods


---  
 

 
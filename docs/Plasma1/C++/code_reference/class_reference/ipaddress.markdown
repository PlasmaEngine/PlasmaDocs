 `Meta`

(NOTE) IPv4/IPv6 network host identifier Provided for convenience Note: This class is not slice-able, it has extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#clear-void)|[ Hash](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#hash-plasma-engine-documen)|SocketAddress| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#ipaddress-void)|[ Host](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#host-plasma-engine-documen)| | |
| |[ InternetProtocol](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#internetprotocol-plasma-en)| | |
| |[ IsValid](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#isvalid-plasma-engine-docu)| | |
| |[ Port](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#port-plasma-engine-documen)| | |
| |[ PortString](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#portstring-plasma-engine-d)| | |
| |[ String](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown#string-plasma-engine-docum)| | |


 #  Properties


---  
 #  Hash : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Hash : Integer


---  
 #  Host : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> Returns the valid IP address host as a numeric string, else String()
> ``` lang=cpp, name=Lightning
> var Host : String


---  
 #  InternetProtocol : [InternetProtocol](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#internetprotocol)

 `read-only`

> Returns the valid IP address protocol version, else InternetProtocol::Unspecified.
> ``` lang=cpp, name=Lightning
> var InternetProtocol : InternetProtocol


---  
 #  IsValid : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if this is a non-empty IPv4/IPv6 address, else false.
> ``` lang=cpp, name=Lightning
> var IsValid : Boolean


---  
 #  Port : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> Returns the valid IP address port, else 0.
> ``` lang=cpp, name=Lightning
> var Port : Integer


---  
 #  PortString : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Returns the valid IP address port as a numeric string, else String()
> ``` lang=cpp, name=Lightning
> var PortString : String


---  
 #  String : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Returns the valid IP address as a numeric "host:port" string, else String()
> ``` lang=cpp, name=Lightning
> var String : String


---  
 #  Methods


---  
 #  Clear : Void

> Clears the IP address.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IpAddress()
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Copy Constructors.
> |Name|Type|Description|
> |---|---|---|
> |rhs|[ipaddress](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ipaddress.markdown)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(rhs : IpAddress)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |port|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(host : String, port : Integer)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |port|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |internetProtocol|[InternetProtocol](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#internetprotocol)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(host : String, port : Integer, internetProtocol : InternetProtocol)
> ``` 


---  
 

 
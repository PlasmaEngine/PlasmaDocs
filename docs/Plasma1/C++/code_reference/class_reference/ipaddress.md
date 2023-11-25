 `Meta`

(NOTE) IPv4/IPv6 network host identifier Provided for convenience Note: This class is not slice-able, it has extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#clear-void)|[ Hash](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#hash-plasma-engine-documen)|SocketAddress| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#ipaddress-void)|[ Host](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#host-plasma-engine-documen)| | |
| |[ InternetProtocol](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#internetprotocol-plasma-en)| | |
| |[ IsValid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#isvalid-plasma-engine-docu)| | |
| |[ Port](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#port-plasma-engine-documen)| | |
| |[ PortString](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#portstring-plasma-engine-d)| | |
| |[ String](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md#string-plasma-engine-docum)| | |


 #  Properties


---  
 #  Hash : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Hash : Integer


---  
 #  Host : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Returns the valid IP address host as a numeric string, else String()
> ``` lang=cpp, name=Lightning
> var Host : String


---  
 #  InternetProtocol : [InternetProtocol](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#internetprotocol)

 `read-only`

> Returns the valid IP address protocol version, else InternetProtocol::Unspecified.
> ``` lang=cpp, name=Lightning
> var InternetProtocol : InternetProtocol


---  
 #  IsValid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if this is a non-empty IPv4/IPv6 address, else false.
> ``` lang=cpp, name=Lightning
> var IsValid : Boolean


---  
 #  Port : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Returns the valid IP address port, else 0.
> ``` lang=cpp, name=Lightning
> var Port : Integer


---  
 #  PortString : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the valid IP address port as a numeric string, else String()
> ``` lang=cpp, name=Lightning
> var PortString : String


---  
 #  String : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

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
> |rhs|[ipaddress](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ipaddress.md)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(rhs : IpAddress)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |port|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(host : String, port : Integer)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |port|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |internetProtocol|[InternetProtocol](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#internetprotocol)| |
> ``` lang=cpp, name=Lightning
> function IpAddress(host : String, port : Integer, internetProtocol : InternetProtocol)
> ``` 


---  
 

 
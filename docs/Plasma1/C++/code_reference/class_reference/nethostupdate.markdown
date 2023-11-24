 `Event` `Networking`



(NOTE) Dispatched when a host discovery operation update occurs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Host](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostupdate.markdown#host-plasma-engine-documen)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ Network](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostupdate.markdown#network-plasma-engine-docu)| | |
| |[ RefreshResult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostupdate.markdown#refreshresult-plasma-engin)| | |
| |[ ResponseTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethostupdate.markdown#responsetime-plasma-engine)| | |


 #  Properties


---  
 #  Host : [nethost](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/nethost.markdown)

 `read-only`

> Host discovered or refreshed (will contain the first host updated if this is a list update).
> ``` lang=cpp, name=Lightning
> var Host : NetHost


---  
 #  Network : [Network](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#network)

 `read-only`

> Operation target network.
> ``` lang=cpp, name=Lightning
> var Network : Network


---  
 #  RefreshResult : [NetRefreshResult](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#netrefreshresult)

 `read-only`

> Whether or not the operation completed successfully.
> ``` lang=cpp, name=Lightning
> var RefreshResult : NetRefreshResult


---  
 #  ResponseTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Operation response time (from request to completion).
> ``` lang=cpp, name=Lightning
> var ResponseTime : Real


---  
 #  Methods


---  
 

 
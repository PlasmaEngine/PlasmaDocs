 `Event` `Networking`



(NOTE) Dispatched when a host discovery operation update occurs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Host](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethostupdate.markdown#host-plasma-engine-documen)|[event](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ Network](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethostupdate.markdown#network-plasma-engine-docu)| | |
| |[ RefreshResult](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethostupdate.markdown#refreshresult-plasma-engin)| | |
| |[ ResponseTime](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethostupdate.markdown#responsetime-plasma-engine)| | |


 #  Properties


---  
 #  Host : [nethost](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/nethost.markdown)

 `read-only`

> Host discovered or refreshed (will contain the first host updated if this is a list update).
> ``` lang=cpp, name=Lightning
> var Host : NetHost


---  
 #  Network : [Network](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#network)

 `read-only`

> Operation target network.
> ``` lang=cpp, name=Lightning
> var Network : Network


---  
 #  RefreshResult : [NetRefreshResult](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#netrefreshresult)

 `read-only`

> Whether or not the operation completed successfully.
> ``` lang=cpp, name=Lightning
> var RefreshResult : NetRefreshResult


---  
 #  ResponseTime : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Operation response time (from request to completion).
> ``` lang=cpp, name=Lightning
> var ResponseTime : Real


---  
 #  Methods


---  
 

 
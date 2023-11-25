 `Component` `Networking`



(NOTE) Network Space. Manages the replication of a single space on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netspace.md#netspace-void)|[ NetObjectCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netspace.md#netobjectcount-plasma-engi)|[netobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md)| |
| |[ NetUserCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netspace.md#netusercount-plasma-engine)| | |


 #  Properties


---  
 #  NetObjectCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the number of net objects in this space (but not including the net space itself).
> ``` lang=cpp, name=Lightning
> var NetObjectCount : Integer


---  
 #  NetUserCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the number of net users in this space.
> ``` lang=cpp, name=Lightning
> var NetUserCount : Integer


---  
 #  Methods


---  
 #  NetSpace : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function NetSpace()
> ``` 


---  
 

 
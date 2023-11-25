 `Component` `Networking`



(NOTE) Network User. Manages the replication of a single negotiated user on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddedByPeer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#addedbypeer-plasma-engine)|[ AddedByMyPeer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#addedbymypeer-plasma-engin)|[netobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md)| |
|[ FindOwnedNetObjectByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#findownednetobjectbyname)|[ NetPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#netpeerid-plasma-engine-do)| | |
|[ FindOwnedNetObjectByNameInSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#findownednetobjectbyname)|[ NetUserId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#netuserid-plasma-engine-do)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#netuser-void)|[ OwnedNetObjectCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#ownednetobjectcount-plasma)| | |
|[ ReleaseOwnedNetObjects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#releaseownednetobjects-v)|[ OwnedNetObjects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md#ownednetobjects-plasma-eng)| | |


 #  Properties


---  
 #  AddedByMyPeer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AddedByMyPeer : Boolean


---  
 #  NetPeerId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Adding network peer identifier.
> ``` lang=cpp, name=Lightning
> var NetPeerId : Integer


---  
 #  NetUserId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Network user identifier.
> ``` lang=cpp, name=Lightning
> var NetUserId : Integer


---  
 #  OwnedNetObjectCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the number of net objects owned by this user in all spaces.
> ``` lang=cpp, name=Lightning
> var OwnedNetObjectCount : Integer


---  
 #  OwnedNetObjects : [coghashsetrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/coghashsetrange.md)

 `read-only`

> Returns all net objects owned by this user in all spaces.
> ``` lang=cpp, name=Lightning
> var OwnedNetObjects : CogHashSetRange


---  
 #  Methods


---  
 #  AddedByPeer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the user was added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function AddedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  FindOwnedNetObjectByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Finds a net object with the given name owned by this user in any space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindOwnedNetObjectByName(name : String) : Cog
> ``` 


---  
 #  FindOwnedNetObjectByNameInSpace : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Finds a net object with the given name owned by this user in the specified space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |space|[space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)| |
> ``` lang=cpp, name=Lightning
> function FindOwnedNetObjectByNameInSpace(name : String, space : Space) : Cog
> ``` 


---  
 #  NetUser : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function NetUser()
> ``` 


---  
 #  ReleaseOwnedNetObjects : Void

> [Server/Offline] Releases ownership of all net objects owned by this user in all spaces.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReleaseOwnedNetObjects()
> ``` 


---  
 

 
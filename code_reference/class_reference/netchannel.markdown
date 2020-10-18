 `Networking`



(NOTE) Network Channel. Manages the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetNetProperty](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#getnetproperty-plasma-engi)|[ Authority](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#authority-plasma-engine-do)|[safeid32object](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/safeid32object.markdown)| |
|[ HasNetProperty](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#hasnetproperty-plasma-engi)|[ ChangeFlag](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#changeflag-plasma-engine-d)| | |
|[ ReplicateNow](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#replicatenow-plasma-engine)|[ IsNapping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#isnapping-plasma-engine-do)| | |
|[ TakeNap](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#takenap-void)|[ IsScheduled](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#isscheduled-plasma-engine)| | |
|[ WakeUp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#wakeup-void)|[ LastChangeTimePassed](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#lastchangetimestamp-plasma)| | |
| |[ Name](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#name-plasma-engine-documen)| | |
| |[ NetChannelType](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown#netchanneltype-plasma-engi)| | |


 #  Properties


---  
 #  Authority : [Authority](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#authority)

> Controls which peer has the authority to observe and replicate property changes. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ``` lang=cpp, name=Lightning
> var Authority : Authority


---  
 #  ChangeFlag : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Manual change flag (checked upon manual change observation).
> ``` lang=cpp, name=Lightning
> var ChangeFlag : Boolean


---  
 #  IsNapping : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net channel is currently napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Lightning
> var IsNapping : Boolean


---  
 #  IsScheduled : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if this net channel is scheduled for change observation, else false.
> ``` lang=cpp, name=Lightning
> var IsScheduled : Boolean


---  
 #  LastChangeTimePassed : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Elapsed time passed since this net channel was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Timestamp indicating when this net channel was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimestamp : Real


---  
 #  Name : [string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Net channel name.
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  NetChannelType : [netchanneltype](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchanneltype.markdown)

 `read-only`

> Operating net channel type.
> ``` lang=cpp, name=Lightning
> var NetChannelType : NetChannelType


---  
 #  Methods


---  
 #  GetNetProperty : [netproperty](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netproperty.markdown)

> [Client/Server] Returns the specified net property, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
> |propertyName|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetNetProperty(component : Component, propertyName : String) : NetProperty
> ``` 


---  
 #  HasNetProperty : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> [Client/Server] Returns true if the net object has the specified net property, else false.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
> |propertyName|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function HasNetProperty(component : Component, propertyName : String) : Boolean
> ``` 


---  
 #  ReplicateNow : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Replicates net property changes immediately (only if changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReplicateNow() : Boolean
> ``` 


---  
 #  TakeNap : Void

> Forces the net channel to start napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function TakeNap()
> ``` 


---  
 #  WakeUp : Void

> Forces the net channel to stop napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WakeUp()
> ``` 


---  
 

 
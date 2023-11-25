 `Networking`



(NOTE) Network Channel Type. Configures the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#resetconfig-void)|[ AcceptIncomingChanges](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#acceptincomingchanges-ze)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.md)| |
|[ SetConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#setconfig-void)|[ AccurateTimestampOnChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#accuratetimestamponchang)| | |
| |[ AllowNapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#allownapping-plasma-engine)| | |
| |[ AllowRelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#allowrelay-plasma-engine-d)| | |
| |[ AuthorityDefault](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#authoritydefault-plasma-en)| | |
| |[ AuthorityMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#authoritymode-plasma-engin)| | |
| |[ AwakeDetectionInterval](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#awakedetectioninterval-z)| | |
| |[ AwakeDuration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#awakeduration-plasma-engin)| | |
| |[ DetectionMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#detectionmode-plasma-engin)| | |
| |[ DetectOutgoingChanges](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#detectoutgoingchanges-ze)| | |
| |[ EventOnIncomingPropertyChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#eventonincomingpropertyc)| | |
| |[ EventOnOutgoingPropertyChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#eventonoutgoingpropertyc)| | |
| |[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#name-plasma-engine-documen)| | |
| |[ NapDetectionInterval](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#napdetectioninterval-zer)| | |
| |[ ReliabilityMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#reliabilitymode-plasma-eng)| | |
| |[ ReplicateOnOffline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#replicateonoffline-plasma)| | |
| |[ ReplicateOnOnline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#replicateononline-plasma-e)| | |
| |[ SerializationMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#serializationmode-plasma-e)| | |
| |[ TransferMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchanneltype.md#transfermode-plasma-engine)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels should accept incoming changes.
> ``` lang=cpp, name=Lightning
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net channel will serialize an accurate timestamp value when changed, or will instead accept an estimated timestamp value. (This setting may be overridden for net channels belonging to a specific net object by enabling the corresponding net object setting)
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnChange : Boolean


---  
 #  AllowNapping : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Lightning
> var AllowNapping : Boolean


---  
 #  AllowRelay : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels will have their changes immediately broadcast to all relevant, incidental peers (if any) once received. (Enabling this allows a server to automatically relay client authoritative changes to other clients, otherwise this must be done manually using NetChannel::ReplicateNow)
> ``` lang=cpp, name=Lightning
> var AllowRelay : Boolean


---  
 #  AuthorityDefault : [Authority](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#authority)

> Controls which peer has the authority to observe and replicate property changes on each net channel by default. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ``` lang=cpp, name=Lightning
> var AuthorityDefault : Authority


---  
 #  AuthorityMode : [AuthorityMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#authoritymode)

> Controls when net channels can modify their change authority. (Dynamic: Authority may be modified at any time, even after a net object is brought online) (Fixed: Authority may be modified only before a net object is brought online) (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var AuthorityMode : AuthorityMode


---  
 #  AwakeDetectionInterval : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Controls the frame interval in which awake net channels are observed for changes. (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var AwakeDetectionInterval : Integer


---  
 #  AwakeDuration : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Controls the frame duration following the last detected change in which net channels are considered actively changing and will be kept awake.
> ``` lang=cpp, name=Lightning
> var AwakeDuration : Integer


---  
 #  DetectionMode : [DetectionMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#detectionmode)

> Controls how net channel changes are detected. (Assume: Assumes something has changed) (Manual: Detects changes manually using change flags) (Automatic: Detects changes automatically using comparisons) (Manumatic: Detects changes manually using change flags and automatically using comparisons)
> ``` lang=cpp, name=Lightning
> var DetectionMode : DetectionMode


---  
 #  DetectOutgoingChanges : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels should detect outgoing changes.
> ``` lang=cpp, name=Lightning
> var DetectOutgoingChanges : Boolean


---  
 #  EventOnIncomingPropertyChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelIncomingPropertyChange when an incoming net property change is accepted.
> ``` lang=cpp, name=Lightning
> var EventOnIncomingPropertyChange : Boolean


---  
 #  EventOnOutgoingPropertyChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelOutgoingPropertyChange when an outgoing net property change is detected.
> ``` lang=cpp, name=Lightning
> var EventOnOutgoingPropertyChange : Boolean


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Net channel type name.
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  NapDetectionInterval : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Controls the frame interval in which napping net channels are observed for changes. (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var NapDetectionInterval : Integer


---  
 #  ReliabilityMode : [ReliabilityMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#reliabilitymode)

> Controls whether or not net channel changes will be retransmitted should they get lost over the network. (Unreliable: Lost changes are not retransmitted) (Reliable: Lost changes are retransmitted)
> ``` lang=cpp, name=Lightning
> var ReliabilityMode : ReliabilityMode


---  
 #  ReplicateOnOffline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object goes offline. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOffline event. (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var ReplicateOnOffline : Boolean


---  
 #  ReplicateOnOnline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object comes online. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOnline event. (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var ReplicateOnOnline : Boolean


---  
 #  SerializationMode : [SerializationMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#serializationmode)

> Controls how net channels are serialized. (All: Serialize all net properties) (Changed: Serialize only net properties that have changed, using bit flags in between) (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var SerializationMode : SerializationMode


---  
 #  TransferMode : [TransferMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#transfermode)

> Controls how net channel changes are to be ordered and released once received. (Immediate: Changes are released immediately once received, including late changes) (Sequenced: Changes are released immediately once received, discarding late changes) (Ordered: Changes are released immediately once preceding late changes have been received; forces all changes to be sent reliably) (Cannot be modified at game runtime)
> ``` lang=cpp, name=Lightning
> var TransferMode : TransferMode


---  
 #  Methods


---  
 #  ResetConfig : Void

> Resets all configuration settings.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ResetConfig()
> ``` 


---  
 #  SetConfig : Void

> Sets all configuration settings according to the specified NetChannelConfig resource.
> |Name|Type|Description|
> |---|---|---|
> |netChannelConfig|[netchannelconfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelconfig.md)| |
> ``` lang=cpp, name=Lightning
> function SetConfig(netChannelConfig : NetChannelConfig)
> ``` 


---  
 

 
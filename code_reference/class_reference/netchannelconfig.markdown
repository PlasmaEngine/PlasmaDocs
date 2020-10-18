 `Resource` `Networking`



(NOTE) Network Channel Configuration. Defines a configuration for the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AcceptIncomingChanges](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#acceptincomingchanges-ze)|[dataresource](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dataresource.markdown)| |
| |[ AccurateTimestampOnChange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#accuratetimestamponchang)| | |
| |[ AllowNapping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#allownapping-plasma-engine)| | |
| |[ AllowRelay](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#allowrelay-plasma-engine-d)| | |
| |[ AuthorityDefault](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#authoritydefault-plasma-en)| | |
| |[ AuthorityMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#authoritymode-plasma-engin)| | |
| |[ AwakeDetectionInterval](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#awakedetectioninterval-z)| | |
| |[ AwakeDuration](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#awakeduration-plasma-engin)| | |
| |[ DetectionMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#detectionmode-plasma-engin)| | |
| |[ DetectOutgoingChanges](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#detectoutgoingchanges-ze)| | |
| |[ EventOnIncomingPropertyChange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#eventonincomingpropertyc)| | |
| |[ EventOnOutgoingPropertyChange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#eventonoutgoingpropertyc)| | |
| |[ NapDetectionInterval](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#napdetectioninterval-zer)| | |
| |[ ReliabilityMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#reliabilitymode-plasma-eng)| | |
| |[ ReplicateOnOffline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#replicateonoffline-plasma)| | |
| |[ ReplicateOnOnline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#replicateononline-plasma-e)| | |
| |[ SerializationMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#serializationmode-plasma-e)| | |
| |[ TransferMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown#transfermode-plasma-engine)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels should accept incoming changes.
> ``` lang=cpp, name=Lightning
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net channel will serialize an accurate timestamp value when changed, or will instead accept an estimated timestamp value. (This setting may be overridden for net channels belonging to a specific net object by enabling the corresponding net object setting)
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnChange : Boolean


---  
 #  AllowNapping : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Lightning
> var AllowNapping : Boolean


---  
 #  AllowRelay : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels will have their changes immediately broadcast to all relevant, incidental peers (if any) once received. (Enabling this allows a server to automatically relay client authoritative changes to other clients, otherwise this must be done manually using NetChannel::ReplicateNow)
> ``` lang=cpp, name=Lightning
> var AllowRelay : Boolean


---  
 #  AuthorityDefault : [Authority](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#authority)

> Controls which peer has the authority to observe and replicate property changes on each net channel by default. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ``` lang=cpp, name=Lightning
> var AuthorityDefault : Authority


---  
 #  AuthorityMode : [AuthorityMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#authoritymode)

> Controls when net channels can modify their change authority. (Dynamic: Authority may be modified at any time, even after a net object is brought online) (Fixed: Authority may be modified only before a net object is brought online)
> ``` lang=cpp, name=Lightning
> var AuthorityMode : AuthorityMode


---  
 #  AwakeDetectionInterval : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Controls the frame interval in which awake net channels are observed for changes.
> ``` lang=cpp, name=Lightning
> var AwakeDetectionInterval : Integer


---  
 #  AwakeDuration : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Controls the frame duration following the last detected change in which net channels are considered actively changing and will be kept awake.
> ``` lang=cpp, name=Lightning
> var AwakeDuration : Integer


---  
 #  DetectionMode : [DetectionMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#detectionmode)

> Controls how net channel changes are detected. (Assume: Assumes something has changed) (Manual: Detects changes manually using change flags) (Automatic: Detects changes automatically using comparisons) (Manumatic: Detects changes manually using change flags and automatically using comparisons)
> ``` lang=cpp, name=Lightning
> var DetectionMode : DetectionMode


---  
 #  DetectOutgoingChanges : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels should detect outgoing changes.
> ``` lang=cpp, name=Lightning
> var DetectOutgoingChanges : Boolean


---  
 #  EventOnIncomingPropertyChange : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels should dispatch NetChannelIncomingPropertyChange when an incoming net property change is accepted.
> ``` lang=cpp, name=Lightning
> var EventOnIncomingPropertyChange : Boolean


---  
 #  EventOnOutgoingPropertyChange : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels should dispatch NetChannelOutgoingPropertyChange when an outgoing net property change is detected.
> ``` lang=cpp, name=Lightning
> var EventOnOutgoingPropertyChange : Boolean


---  
 #  NapDetectionInterval : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Controls the frame interval in which napping net channels are observed for changes.
> ``` lang=cpp, name=Lightning
> var NapDetectionInterval : Integer


---  
 #  ReliabilityMode : [ReliabilityMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#reliabilitymode)

> Controls whether or not net channel changes will be retransmitted should they get lost over the network. (Unreliable: Lost changes are not retransmitted) (Reliable: Lost changes are retransmitted)
> ``` lang=cpp, name=Lightning
> var ReliabilityMode : ReliabilityMode


---  
 #  ReplicateOnOffline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net channel will be replicated when the net object goes offline. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOffline event.
> ``` lang=cpp, name=Lightning
> var ReplicateOnOffline : Boolean


---  
 #  ReplicateOnOnline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net channel will be replicated when the net object comes online. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOnline event.
> ``` lang=cpp, name=Lightning
> var ReplicateOnOnline : Boolean


---  
 #  SerializationMode : [SerializationMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#serializationmode)

> Controls how net channels are serialized. (All: Serialize all net properties) (Changed: Serialize only net properties that have changed, using bit flags in between)
> ``` lang=cpp, name=Lightning
> var SerializationMode : SerializationMode


---  
 #  TransferMode : [TransferMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#transfermode)

> Controls how net channel changes are to be ordered and released once received. (Immediate: Changes are released immediately once received, including late changes) (Sequenced: Changes are released immediately once received, discarding late changes) (Ordered: Changes are released immediately once preceding late changes have been received; forces all changes to be sent reliably)
> ``` lang=cpp, name=Lightning
> var TransferMode : TransferMode


---  
 #  Methods


---  
 

 
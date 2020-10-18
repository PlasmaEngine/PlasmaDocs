 `Component` `Networking`



(NOTE) Network Object. Manages the replication of a single object on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchBroadcast](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#dispatchbroadcast-void)|[ AcceptIncomingChanges](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#acceptincomingchanges-ze)|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)|[netpeer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpeer.markdown)|
|[ DispatchLocal](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#dispatchlocal-void)|[ AccurateTimestampOnChange](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#accuratetimestamponchang)| |[netspace](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netspace.markdown)|
|[ DispatchLocalAndBroadcast](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#dispatchlocalandbroadcas)|[ AccurateTimestampOnOffline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#accuratetimestamponoffli)| |[netuser](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netuser.markdown)|
|[ DispatchLocalAndRemote](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#dispatchlocalandremote-v)|[ AccurateTimestampOnOnline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#accuratetimestampononlin)| | |
|[ DispatchRemote](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#dispatchremote-void)|[ AllowNapping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#allownapping-plasma-engine)| | |
|[ Forget](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#forget-plasma-engine-docum)|[ AutomaticChannel](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#automaticchannel-plasma-en)| | |
|[ GetNetChannel](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#getnetchannel-plasma-engin)|[ DetectOutgoingChanges](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#detectoutgoingchanges-ze)| | |
|[ HasNetChannel](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#hasnetchannel-plasma-engin)|[ IsClient](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isclient-plasma-engine-doc)| | |
|[ IsOwnedByPeer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isownedbypeer-plasma-engin)|[ IsClientAndMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isclientandmine-plasma-eng)| | |
|[ IsOwnedByUser](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isownedbyuser-plasma-engin)|[ IsClientButNotMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isclientbutnotmine-plasma)| | |
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netobject-void)|[ IsClientOrOffline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isclientoroffline-plasma-e)| | |
|[ ReplicateNow](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#replicatenow-plasma-engine)|[ IsClientOrServer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isclientorserver-plasma-en)| | |
|[ SelectRemote](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#selectremote-plasma-engine)|[ IsMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#ismine-plasma-engine-docum)| | |
|[ SetNetUserOwnerDown](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#setnetuserownerdown-void)|[ IsNapping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isnapping-plasma-engine-do)| | |
|[ SetNetUserOwnerUp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#setnetuserownerup-void)|[ IsNotMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isnotmine-plasma-engine-do)| | |
|[ TakeNap](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#takenap-void)|[ IsNotOwnedByAUser](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isnotownedbyauser-plasma-e)| | |
|[ WakeUp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#wakeup-void)|[ IsOffline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isoffline-plasma-engine-do)| | |
| |[ IsOfflineAndMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isofflineandmine-plasma-en)| | |
| |[ IsOfflineButNotMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isofflinebutnotmine-plasma)| | |
| |[ IsOnline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isonline-plasma-engine-doc)| | |
| |[ IsOwnedByAUser](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isownedbyauser-plasma-engi)| | |
| |[ IsServer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isserver-plasma-engine-doc)| | |
| |[ IsServerAndMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isserverandmine-plasma-eng)| | |
| |[ IsServerButNotMine](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isserverbutnotmine-plasma)| | |
| |[ IsServerOrOffline](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#isserveroroffline-plasma-e)| | |
| |[ LastChangeTimePassed](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#lastchangetimestamp-plasma)| | |
| |[ NetObjectId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netobjectid-plasma-engine)| | |
| |[ NetPropertyInfos](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netpropertyinfos-plasma-en)| | |
| |[ NetUserOwner](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netuserowner-plasma-engine)| | |
| |[ NetUserOwnerPath](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netuserownerpath-plasma-en)| | |
| |[ NetUserOwnerPeerId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netuserownerpeerid-plasma)| | |
| |[ NetUserOwnerUserId](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#netuserowneruserid-plasma)| | |
| |[ OfflineTimePassed](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#offlinetimepassed-plasma-e)| | |
| |[ OfflineTimestamp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#offlinetimestamp-plasma-en)| | |
| |[ OnlineTimePassed](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#onlinetimepassed-plasma-en)| | |
| |[ OnlineTimestamp](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#onlinetimestamp-plasma-eng)| | |
| |[ Role](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netobject.markdown#role-plasma-engine-documen)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels on this net object may accept incoming changes.
> ``` lang=cpp, name=Lightning
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net object will serialize an accurate timestamp value when changed (on any net channel), or will instead accept an estimated timestamp value. (Enabling this will override the corresponding net channel type setting for all net channels added to this net object)
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnChange : Boolean


---  
 #  AccurateTimestampOnOffline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net object will serialize an accurate timestamp value when taken offline, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnOffline : Boolean


---  
 #  AccurateTimestampOnOnline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not the net object will serialize an accurate timestamp value when brought online, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnOnline : Boolean


---  
 #  AllowNapping : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels on this net object may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Lightning
> var AllowNapping : Boolean


---  
 #  AutomaticChannel : [netchannelconfig](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannelconfig.markdown)

> Returns the automatic net channel configuration resource (assigned to net properties unless another channel is specified).
> ``` lang=cpp, name=Lightning
> var AutomaticChannel : NetChannelConfig


---  
 #  DetectOutgoingChanges : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Controls whether or not net channels on this net object may detect outgoing changes.
> ``` lang=cpp, name=Lightning
> var DetectOutgoingChanges : Boolean


---  
 #  IsClient : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is client, else false.
> ``` lang=cpp, name=Lightning
> var IsClient : Boolean


---  
 #  IsClientAndMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is client and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsClientAndMine : Boolean


---  
 #  IsClientButNotMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is client and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsClientButNotMine : Boolean


---  
 #  IsClientOrOffline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is client or offline, else false.
> ``` lang=cpp, name=Lightning
> var IsClientOrOffline : Boolean


---  
 #  IsClientOrServer : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is client or server, else false.
> ``` lang=cpp, name=Lightning
> var IsClientOrServer : Boolean


---  
 #  IsMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsMine : Boolean


---  
 #  IsNapping : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if all net channels on this net object are napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Lightning
> var IsNapping : Boolean


---  
 #  IsNotMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsNotMine : Boolean


---  
 #  IsNotOwnedByAUser : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net object is not conceptually owned by a user, else false.
> ``` lang=cpp, name=Lightning
> var IsNotOwnedByAUser : Boolean


---  
 #  IsOffline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is offline, else false.
> ``` lang=cpp, name=Lightning
> var IsOffline : Boolean


---  
 #  IsOfflineAndMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsOfflineAndMine : Boolean


---  
 #  IsOfflineButNotMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsOfflineButNotMine : Boolean


---  
 #  IsOnline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net object is online, else false.
> ``` lang=cpp, name=Lightning
> var IsOnline : Boolean


---  
 #  IsOwnedByAUser : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if the net object is conceptually owned by a user, else false.
> ``` lang=cpp, name=Lightning
> var IsOwnedByAUser : Boolean


---  
 #  IsServer : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is server, else false.
> ``` lang=cpp, name=Lightning
> var IsServer : Boolean


---  
 #  IsServerAndMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is server and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsServerAndMine : Boolean


---  
 #  IsServerButNotMine : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is server and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsServerButNotMine : Boolean


---  
 #  IsServerOrOffline : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns true if our open peer's network role is server or offline, else false.
> ``` lang=cpp, name=Lightning
> var IsServerOrOffline : Boolean


---  
 #  LastChangeTimePassed : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Elapsed time passed since this net object was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Timestamp indicating when this net object was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimestamp : Real


---  
 #  NetObjectId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns the net object ID (set if the net object is live), else 0.
> ``` lang=cpp, name=Lightning
> var NetObjectId : Integer


---  
 #  NetPropertyInfos : [netpropertyinfos](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netpropertyinfos.markdown)

> Net property infos added through the property grid.
> ``` lang=cpp, name=Lightning
> var NetPropertyInfos : NetPropertyInfos


---  
 #  NetUserOwner : [cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

> Returns the network user this object conceptually belongs to, else nullptr.
> ``` lang=cpp, name=Lightning
> var NetUserOwner : Cog


---  
 #  NetUserOwnerPath : [cogpath](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cogpath.markdown)

 `read-only`

> Path to the network user this object conceptually belongs to, else empty cog path.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerPath : CogPath


---  
 #  NetUserOwnerPeerId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns the network peer identifier of the peer who added the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerPeerId : Integer


---  
 #  NetUserOwnerUserId : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns the network user identifier of the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerUserId : Integer


---  
 #  OfflineTimePassed : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Elapsed time passed since this net object was taken offline, else 0.
> ``` lang=cpp, name=Lightning
> var OfflineTimePassed : Real


---  
 #  OfflineTimestamp : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Timestamp indicating when this net object was taken offline, else 0.
> ``` lang=cpp, name=Lightning
> var OfflineTimestamp : Real


---  
 #  OnlineTimePassed : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Elapsed time passed since this net object was brought online, else 0.
> ``` lang=cpp, name=Lightning
> var OnlineTimePassed : Real


---  
 #  OnlineTimestamp : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Timestamp indicating when this net object was brought online, else 0.
> ``` lang=cpp, name=Lightning
> var OnlineTimestamp : Real


---  
 #  Role : [NetRole](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#netrole)

 `read-only`

> Returns our open peer's network role (client, server, offline), else Role::Unspecified.
> ``` lang=cpp, name=Lightning
> var Role : NetRole


---  
 #  Methods


---  
 #  DispatchBroadcast : Void

> Dispatches the net event on the net object for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocal : Void

> Dispatches the net event on the net object for the local peer.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocal(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndBroadcast : Void

> Dispatches the net event on the net object for the local peer and for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocalAndBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndRemote : Void

> Dispatches the net event on the net object for the local peer and for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
> |netPeerId|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocalAndRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  DispatchRemote : Void

> Dispatches the net event on the net object for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[event](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
> |netPeerId|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function DispatchRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  Forget : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> [Client] Forgets the online net object locally. [Server] Forgets the online net object locally and remotely for all relevant peers. Effectively removes the net object from the network system without destroying it. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Forget() : Boolean
> ``` 


---  
 #  GetNetChannel : [netchannel](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/netchannel.markdown)

> [Client/Server] Returns the specified net channel, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetNetChannel(netChannelName : String) : NetChannel
> ``` 


---  
 #  HasNetChannel : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> [Client/Server] Returns true if the net object has the specified net channel, else false.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function HasNetChannel(netChannelName : String) : Boolean
> ``` 


---  
 #  IsOwnedByPeer : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the net object is conceptually owned by a user added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsOwnedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  IsOwnedByUser : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the net object is conceptually owned by the specified user, else false.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsOwnedByUser(cog : Cog) : Boolean
> ``` 


---  
 #  NetObject : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function NetObject()
> ``` 


---  
 #  ReplicateNow : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> [Client/Server] Replicates all net channels' property changes immediately (only where changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReplicateNow() : Boolean
> ``` 


---  
 #  SelectRemote : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> [Client/Server] Selects the remote net object on the first opposite-role peer found running in another game session instance on the engine. Will fail if the net object is not online, or not found remotely. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SelectRemote() : Boolean
> ``` 


---  
 #  SetNetUserOwnerDown : Void

> [Server/Offline] Sets the owning network user on this object and down the tree on all children recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetNetUserOwnerDown(cog : Cog)
> ``` 


---  
 #  SetNetUserOwnerUp : Void

> [Server/Offline] Sets the owning network user on this object and up the tree on each parent recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetNetUserOwnerUp(cog : Cog)
> ``` 


---  
 #  TakeNap : Void

> Forces all net channels on this net object to start napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function TakeNap()
> ``` 


---  
 #  WakeUp : Void

> Forces all net channels on this net object to stop napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WakeUp()
> ``` 


---  
 

 
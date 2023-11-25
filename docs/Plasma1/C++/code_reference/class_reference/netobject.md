 `Component` `Networking`



(NOTE) Network Object. Manages the replication of a single object on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchBroadcast](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#dispatchbroadcast-void)|[ AcceptIncomingChanges](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#acceptincomingchanges-ze)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)|[netpeer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpeer.md)|
|[ DispatchLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#dispatchlocal-void)|[ AccurateTimestampOnChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#accuratetimestamponchang)| |[netspace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netspace.md)|
|[ DispatchLocalAndBroadcast](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#dispatchlocalandbroadcas)|[ AccurateTimestampOnOffline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#accuratetimestamponoffli)| |[netuser](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuser.md)|
|[ DispatchLocalAndRemote](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#dispatchlocalandremote-v)|[ AccurateTimestampOnOnline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#accuratetimestampononlin)| | |
|[ DispatchRemote](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#dispatchremote-void)|[ AllowNapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#allownapping-plasma-engine)| | |
|[ Forget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#forget-plasma-engine-docum)|[ AutomaticChannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#automaticchannel-plasma-en)| | |
|[ GetNetChannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#getnetchannel-plasma-engin)|[ DetectOutgoingChanges](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#detectoutgoingchanges-ze)| | |
|[ HasNetChannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#hasnetchannel-plasma-engin)|[ IsClient](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isclient-plasma-engine-doc)| | |
|[ IsOwnedByPeer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isownedbypeer-plasma-engin)|[ IsClientAndMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isclientandmine-plasma-eng)| | |
|[ IsOwnedByUser](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isownedbyuser-plasma-engin)|[ IsClientButNotMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isclientbutnotmine-plasma)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netobject-void)|[ IsClientOrOffline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isclientoroffline-plasma-e)| | |
|[ ReplicateNow](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#replicatenow-plasma-engine)|[ IsClientOrServer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isclientorserver-plasma-en)| | |
|[ SelectRemote](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#selectremote-plasma-engine)|[ IsMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#ismine-plasma-engine-docum)| | |
|[ SetNetUserOwnerDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#setnetuserownerdown-void)|[ IsNapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isnapping-plasma-engine-do)| | |
|[ SetNetUserOwnerUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#setnetuserownerup-void)|[ IsNotMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isnotmine-plasma-engine-do)| | |
|[ TakeNap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#takenap-void)|[ IsNotOwnedByAUser](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isnotownedbyauser-plasma-e)| | |
|[ WakeUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#wakeup-void)|[ IsOffline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isoffline-plasma-engine-do)| | |
| |[ IsOfflineAndMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isofflineandmine-plasma-en)| | |
| |[ IsOfflineButNotMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isofflinebutnotmine-plasma)| | |
| |[ IsOnline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isonline-plasma-engine-doc)| | |
| |[ IsOwnedByAUser](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isownedbyauser-plasma-engi)| | |
| |[ IsServer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isserver-plasma-engine-doc)| | |
| |[ IsServerAndMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isserverandmine-plasma-eng)| | |
| |[ IsServerButNotMine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isserverbutnotmine-plasma)| | |
| |[ IsServerOrOffline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#isserveroroffline-plasma-e)| | |
| |[ LastChangeTimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#lastchangetimestamp-plasma)| | |
| |[ NetObjectId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netobjectid-plasma-engine)| | |
| |[ NetPropertyInfos](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netpropertyinfos-plasma-en)| | |
| |[ NetUserOwner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netuserowner-plasma-engine)| | |
| |[ NetUserOwnerPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netuserownerpath-plasma-en)| | |
| |[ NetUserOwnerPeerId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netuserownerpeerid-plasma)| | |
| |[ NetUserOwnerUserId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#netuserowneruserid-plasma)| | |
| |[ OfflineTimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#offlinetimepassed-plasma-e)| | |
| |[ OfflineTimestamp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#offlinetimestamp-plasma-en)| | |
| |[ OnlineTimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#onlinetimepassed-plasma-en)| | |
| |[ OnlineTimestamp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#onlinetimestamp-plasma-eng)| | |
| |[ Role](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netobject.md#role-plasma-engine-documen)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels on this net object may accept incoming changes.
> ``` lang=cpp, name=Lightning
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when changed (on any net channel), or will instead accept an estimated timestamp value. (Enabling this will override the corresponding net channel type setting for all net channels added to this net object)
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnChange : Boolean


---  
 #  AccurateTimestampOnOffline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when taken offline, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnOffline : Boolean


---  
 #  AccurateTimestampOnOnline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when brought online, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Lightning
> var AccurateTimestampOnOnline : Boolean


---  
 #  AllowNapping : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels on this net object may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Lightning
> var AllowNapping : Boolean


---  
 #  AutomaticChannel : [netchannelconfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelconfig.md)

> Returns the automatic net channel configuration resource (assigned to net properties unless another channel is specified).
> ``` lang=cpp, name=Lightning
> var AutomaticChannel : NetChannelConfig


---  
 #  DetectOutgoingChanges : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Controls whether or not net channels on this net object may detect outgoing changes.
> ``` lang=cpp, name=Lightning
> var DetectOutgoingChanges : Boolean


---  
 #  IsClient : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client, else false.
> ``` lang=cpp, name=Lightning
> var IsClient : Boolean


---  
 #  IsClientAndMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsClientAndMine : Boolean


---  
 #  IsClientButNotMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsClientButNotMine : Boolean


---  
 #  IsClientOrOffline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or offline, else false.
> ``` lang=cpp, name=Lightning
> var IsClientOrOffline : Boolean


---  
 #  IsClientOrServer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or server, else false.
> ``` lang=cpp, name=Lightning
> var IsClientOrServer : Boolean


---  
 #  IsMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsMine : Boolean


---  
 #  IsNapping : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if all net channels on this net object are napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Lightning
> var IsNapping : Boolean


---  
 #  IsNotMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsNotMine : Boolean


---  
 #  IsNotOwnedByAUser : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user, else false.
> ``` lang=cpp, name=Lightning
> var IsNotOwnedByAUser : Boolean


---  
 #  IsOffline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline, else false.
> ``` lang=cpp, name=Lightning
> var IsOffline : Boolean


---  
 #  IsOfflineAndMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsOfflineAndMine : Boolean


---  
 #  IsOfflineButNotMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsOfflineButNotMine : Boolean


---  
 #  IsOnline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if the net object is online, else false.
> ``` lang=cpp, name=Lightning
> var IsOnline : Boolean


---  
 #  IsOwnedByAUser : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user, else false.
> ``` lang=cpp, name=Lightning
> var IsOwnedByAUser : Boolean


---  
 #  IsServer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server, else false.
> ``` lang=cpp, name=Lightning
> var IsServer : Boolean


---  
 #  IsServerAndMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsServerAndMine : Boolean


---  
 #  IsServerButNotMine : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Lightning
> var IsServerButNotMine : Boolean


---  
 #  IsServerOrOffline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server or offline, else false.
> ``` lang=cpp, name=Lightning
> var IsServerOrOffline : Boolean


---  
 #  LastChangeTimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimestamp : Real


---  
 #  NetObjectId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the net object ID (set if the net object is live), else 0.
> ``` lang=cpp, name=Lightning
> var NetObjectId : Integer


---  
 #  NetPropertyInfos : [netpropertyinfos](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpropertyinfos.md)

> Net property infos added through the property grid.
> ``` lang=cpp, name=Lightning
> var NetPropertyInfos : NetPropertyInfos


---  
 #  NetUserOwner : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Returns the network user this object conceptually belongs to, else nullptr.
> ``` lang=cpp, name=Lightning
> var NetUserOwner : Cog


---  
 #  NetUserOwnerPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

 `read-only`

> Path to the network user this object conceptually belongs to, else empty cog path.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerPath : CogPath


---  
 #  NetUserOwnerPeerId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the network peer identifier of the peer who added the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerPeerId : Integer


---  
 #  NetUserOwnerUserId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the network user identifier of the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Lightning
> var NetUserOwnerUserId : Integer


---  
 #  OfflineTimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was taken offline, else 0.
> ``` lang=cpp, name=Lightning
> var OfflineTimePassed : Real


---  
 #  OfflineTimestamp : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was taken offline, else 0.
> ``` lang=cpp, name=Lightning
> var OfflineTimestamp : Real


---  
 #  OnlineTimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was brought online, else 0.
> ``` lang=cpp, name=Lightning
> var OnlineTimePassed : Real


---  
 #  OnlineTimestamp : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was brought online, else 0.
> ``` lang=cpp, name=Lightning
> var OnlineTimestamp : Real


---  
 #  Role : [NetRole](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#netrole)

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
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocal : Void

> Dispatches the net event on the net object for the local peer.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocal(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndBroadcast : Void

> Dispatches the net event on the net object for the local peer and for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocalAndBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndRemote : Void

> Dispatches the net event on the net object for the local peer and for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> |netPeerId|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchLocalAndRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  DispatchRemote : Void

> Dispatches the net event on the net object for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> |netPeerId|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  Forget : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> [Client] Forgets the online net object locally. [Server] Forgets the online net object locally and remotely for all relevant peers. Effectively removes the net object from the network system without destroying it. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Forget() : Boolean
> ``` 


---  
 #  GetNetChannel : [netchannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannel.md)

> [Client/Server] Returns the specified net channel, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetNetChannel(netChannelName : String) : NetChannel
> ``` 


---  
 #  HasNetChannel : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> [Client/Server] Returns true if the net object has the specified net channel, else false.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function HasNetChannel(netChannelName : String) : Boolean
> ``` 


---  
 #  IsOwnedByPeer : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the net object is conceptually owned by a user added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function IsOwnedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  IsOwnedByUser : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the net object is conceptually owned by the specified user, else false.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
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
 #  ReplicateNow : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> [Client/Server] Replicates all net channels' property changes immediately (only where changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReplicateNow() : Boolean
> ``` 


---  
 #  SelectRemote : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

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
> |cog|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function SetNetUserOwnerDown(cog : Cog)
> ``` 


---  
 #  SetNetUserOwnerUp : Void

> [Server/Offline] Sets the owning network user on this object and up the tree on each parent recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
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
 

 
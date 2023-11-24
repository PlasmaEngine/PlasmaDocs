 `Event` `Networking`



(NOTE) Dispatched after an outgoing/incoming net channel property change is detected during a particular replication phase.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ChannelName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#channelname-plasma-engine)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ ComponentName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#componentname-plasma-engin)| | |
| |[ Direction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#direction-plasma-engine-do)| | |
| |[ Object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#object-plasma-engine-docum)| | |
| |[ PropertyName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#propertyname-plasma-engine)| | |
| |[ ReplicationPhase](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#replicationphase-plasma-en)| | |
| |[ Timestamp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannelpropertychange.markdown#timestamp-plasma-engine-do)| | |


 #  Properties


---  
 #  ChannelName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The changed net channel.
> ``` lang=cpp, name=Lightning
> var ChannelName : String


---  
 #  ComponentName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The component which declared the changed net property.
> ``` lang=cpp, name=Lightning
> var ComponentName : String


---  
 #  Direction : [TransmissionDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#transmissiondirection)

 `read-only`

> The change direction.
> ``` lang=cpp, name=Lightning
> var Direction : TransmissionDirection


---  
 #  Object : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The changed net object.
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  PropertyName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The changed net property.
> ``` lang=cpp, name=Lightning
> var PropertyName : String


---  
 #  ReplicationPhase : [ReplicationPhase](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#replicationphase)

 `read-only`

> The replication phase.
> ``` lang=cpp, name=Lightning
> var ReplicationPhase : ReplicationPhase


---  
 #  Timestamp : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The time this change occurred.
> ``` lang=cpp, name=Lightning
> var Timestamp : Real


---  
 #  Methods


---  
 

 
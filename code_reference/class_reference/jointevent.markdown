 `Event` `Physics`



(NOTE) Sent out when a joint reaches some condition. Currently sent out when a limit is reached or an impulse's limit is exceeded.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointevent.markdown#joint-plasma-engine-docume)|[event](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/event.markdown)| |
| |[ JointCog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointevent.markdown#jointcog-plasma-engine-doc)| | |
| |[ ObjectA](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointevent.markdown#objecta-plasma-engine-docu)| | |
| |[ ObjectB](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/jointevent.markdown#objectb-plasma-engine-docu)| | |


 #  Properties


---  
 #  Joint : [joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)

 `read-only`

> The Joint that triggered the event.
> ``` lang=cpp, name=Lightning
> var Joint : Joint


---  
 #  JointCog : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> The Cog of the Joint that signaled the event.
> ``` lang=cpp, name=Lightning
> var JointCog : Cog


---  
 #  ObjectA : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> ObjectA on the Joint.
> ``` lang=cpp, name=Lightning
> var ObjectA : Cog


---  
 #  ObjectB : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> ObjectB on the Joint.
> ``` lang=cpp, name=Lightning
> var ObjectB : Cog


---  
 #  Methods


---  
 

 
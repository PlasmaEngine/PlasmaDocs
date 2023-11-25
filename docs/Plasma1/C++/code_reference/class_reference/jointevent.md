 `Event` `Physics`



(NOTE) Sent out when a joint reaches some condition. Currently sent out when a limit is reached or an impulse's limit is exceeded.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointevent.md#joint-plasma-engine-docume)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ JointCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointevent.md#jointcog-plasma-engine-doc)| | |
| |[ ObjectA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointevent.md#objecta-plasma-engine-docu)| | |
| |[ ObjectB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointevent.md#objectb-plasma-engine-docu)| | |


 #  Properties


---  
 #  Joint : [joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)

 `read-only`

> The Joint that triggered the event.
> ``` lang=cpp, name=Lightning
> var Joint : Joint


---  
 #  JointCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The Cog of the Joint that signaled the event.
> ``` lang=cpp, name=Lightning
> var JointCog : Cog


---  
 #  ObjectA : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> ObjectA on the Joint.
> ``` lang=cpp, name=Lightning
> var ObjectA : Cog


---  
 #  ObjectB : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> ObjectB on the Joint.
> ``` lang=cpp, name=Lightning
> var ObjectB : Cog


---  
 #  Methods


---  
 

 
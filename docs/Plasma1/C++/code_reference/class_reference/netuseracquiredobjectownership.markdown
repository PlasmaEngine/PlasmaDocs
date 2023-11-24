 `Event` `Networking`



(NOTE) Dispatched after the net user acquires network ownership of a net object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AcquiredObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuseracquiredobjectownership.markdown#acquiredobject-plasma-engi)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ PreviousNetUserOwner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuseracquiredobjectownership.markdown#previousnetuserowner-zer)| | |


 #  Properties


---  
 #  AcquiredObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The object this user just acquired network ownership of.
> ``` lang=cpp, name=Lightning
> var AcquiredObject : Cog


---  
 #  PreviousNetUserOwner : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The object's previous network user owner.
> ``` lang=cpp, name=Lightning
> var PreviousNetUserOwner : Cog


---  
 #  Methods


---  
 

 
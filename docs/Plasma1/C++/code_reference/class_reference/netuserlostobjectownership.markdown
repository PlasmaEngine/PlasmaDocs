 `Event` `Networking`



(NOTE) Dispatched after the net user loses network ownership of a net object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ CurrentNetUserOwner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuserlostobjectownership.markdown#currentnetuserowner-plasma)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ LostObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netuserlostobjectownership.markdown#lostobject-plasma-engine-d)| | |


 #  Properties


---  
 #  CurrentNetUserOwner : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The object's current network user owner.
> ``` lang=cpp, name=Lightning
> var CurrentNetUserOwner : Cog


---  
 #  LostObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> The object this user just lost network ownership of.
> ``` lang=cpp, name=Lightning
> var LostObject : Cog


---  
 #  Methods


---  
 

 
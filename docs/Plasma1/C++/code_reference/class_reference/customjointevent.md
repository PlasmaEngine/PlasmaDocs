 `Event` `Physics`



(NOTE) Sent by CustomJoint before solving constraints. Used to configure constraints before the physics system begins solving.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Dt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointevent.md#dt-plasma-engine-documenta)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ Owner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointevent.md#owner-plasma-engine-docume)| | |


 #  Properties


---  
 #  Dt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The current frame's delta time. Use to setup the constraint if necessary.
> ``` lang=cpp, name=Lightning
> var Dt : Real


---  
 #  Owner : [customjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md)

> The joint that sent this event.
> ``` lang=cpp, name=Lightning
> var Owner : CustomJoint


---  
 #  Methods


---  
 

 
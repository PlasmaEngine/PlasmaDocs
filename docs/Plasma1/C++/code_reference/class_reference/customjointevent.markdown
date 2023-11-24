 `Event` `Physics`



(NOTE) Sent by CustomJoint before solving constraints. Used to configure constraints before the physics system begins solving.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Dt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointevent.markdown#dt-plasma-engine-documenta)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ Owner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointevent.markdown#owner-plasma-engine-docume)| | |


 #  Properties


---  
 #  Dt : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The current frame's delta time. Use to setup the constraint if necessary.
> ``` lang=cpp, name=Lightning
> var Dt : Real


---  
 #  Owner : [customjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.markdown)

> The joint that sent this event.
> ``` lang=cpp, name=Lightning
> var Owner : CustomJoint


---  
 #  Methods


---  
 

 
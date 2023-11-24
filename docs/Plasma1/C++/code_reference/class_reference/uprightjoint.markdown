 `Component` `Physics`



(NOTE) A joint to keep an object upright. Locks two axes of the objects together but allows free rotation on the plane defined by that axis. This constraint is useful for keeping any object upright. This could also be used to auto correct an object slowly by lowering the max impulse value of the constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.markdown#uprightjoint-void)|[ LocalAxisA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.markdown#localaxisa-plasma-engine-d)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.markdown)| |
| |[ LocalAxisB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.markdown#localaxisb-plasma-engine-d)| | |
| |[ WorldAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.markdown#worldaxis-plasma-engine-do)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object A . 
> ``` lang=cpp, name=Lightning
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object B . 
> ``` lang=cpp, name=Lightning
> var LocalAxisB : Real3


---  
 #  WorldAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The axis in world space that is being rotated about . 
> ``` lang=cpp, name=Lightning
> var WorldAxis : Real3


---  
 #  Methods


---  
 #  UprightJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UprightJoint()
> ``` 


---  
 

 
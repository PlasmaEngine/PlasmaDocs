 `Component` `Physics`



(NOTE) A joint to keep an object upright. Locks two axes of the objects together but allows free rotation on the plane defined by that axis. This constraint is useful for keeping any object upright. This could also be used to auto correct an object slowly by lowering the max impulse value of the constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uprightjoint.markdown#uprightjoint-void)|[ LocalAxisA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uprightjoint.markdown#localaxisa-plasma-engine-d)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/joint.markdown)| |
| |[ LocalAxisB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uprightjoint.markdown#localaxisb-plasma-engine-d)| | |
| |[ WorldAxis](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uprightjoint.markdown#worldaxis-plasma-engine-do)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object A . 
> ``` lang=cpp, name=Lightning
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The locally defined axis on object B . 
> ``` lang=cpp, name=Lightning
> var LocalAxisB : Real3


---  
 #  WorldAxis : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

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
 

 
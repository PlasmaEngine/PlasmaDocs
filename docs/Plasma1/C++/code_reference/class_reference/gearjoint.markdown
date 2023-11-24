 `Component` `Physics`



(NOTE) A gear connects two joints on two objects together. Either joint can be a prismatic or a revolute. A gear ratio is used to bind the two joints together. Limits, motors, and springs should not be used on this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#gearjoint-void)|[ Constant](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#constant-plasma-engine-doc)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/joint.markdown)| |
| |[ JointA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#jointa-plasma-engine-docum)| | |
| |[ JointAPath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#jointapath-plasma-engine-d)| | |
| |[ JointB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#jointb-plasma-engine-docum)| | |
| |[ JointBPath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#jointbpath-plasma-engine-d)| | |
| |[ Ratio](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/gearjoint.markdown#ratio-plasma-engine-docume)| | |


 #  Properties


---  
 #  Constant : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The initial offset of the gear ratio.
> ``` lang=cpp, name=Lightning
> var Constant : Real


---  
 #  JointA : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointA : Cog


---  
 #  JointAPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointAPath : CogPath


---  
 #  JointB : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointB : Cog


---  
 #  JointBPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointBPath : CogPath


---  
 #  Ratio : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The gear ratio that the two constraints are bound with.
> ``` lang=cpp, name=Lightning
> var Ratio : Real


---  
 #  Methods


---  
 #  GearJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GearJoint()
> ``` 


---  
 

 
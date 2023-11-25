 `Component` `Physics`



(NOTE) A gear connects two joints on two objects together. Either joint can be a prismatic or a revolute. A gear ratio is used to bind the two joints together. Limits, motors, and springs should not be used on this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#gearjoint-void)|[ Constant](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#constant-plasma-engine-doc)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
| |[ JointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#jointa-plasma-engine-docum)| | |
| |[ JointAPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#jointapath-plasma-engine-d)| | |
| |[ JointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#jointb-plasma-engine-docum)| | |
| |[ JointBPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#jointbpath-plasma-engine-d)| | |
| |[ Ratio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md#ratio-plasma-engine-docume)| | |


 #  Properties


---  
 #  Constant : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The initial offset of the gear ratio.
> ``` lang=cpp, name=Lightning
> var Constant : Real


---  
 #  JointA : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointA : Cog


---  
 #  JointAPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointAPath : CogPath


---  
 #  JointB : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointB : Cog


---  
 #  JointBPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Lightning
> var JointBPath : CogPath


---  
 #  Ratio : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

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
 

 
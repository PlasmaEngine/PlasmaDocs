 `Component` `Physics`



(NOTE) A PulleyJoint turns two StickJoints into a pulley via a pulley ratio. A PulleyJoint connects the two free objects of two different stick joints. These two objects will then be bound to move together via the formula "length0 + ratio * length1 = 0". Limits, motors and springs should not be used on a pulley.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#pulleyjoint-void)|[ JointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#jointa-plasma-engine-docum)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.markdown)| |
| |[ JointAPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#jointapath-plasma-engine-d)| | |
| |[ JointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#jointb-plasma-engine-docum)| | |
| |[ JointBPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#jointbpath-plasma-engine-d)| | |
| |[ Ratio](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.markdown#ratio-plasma-engine-docume)| | |


 #  Properties


---  
 #  JointA : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> The joint connected to ObjectA that the pulley operates on.
> ``` lang=cpp, name=Lightning
> var JointA : Cog


---  
 #  JointAPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.markdown)

> The joint connected to ObjectA that the pulley operates on.
> ``` lang=cpp, name=Lightning
> var JointAPath : CogPath


---  
 #  JointB : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

> The joint connected to ObjectB that the pulley operates on.
> ``` lang=cpp, name=Lightning
> var JointB : Cog


---  
 #  JointBPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.markdown)

> The joint connected to ObjectB that the pulley operates on.
> ``` lang=cpp, name=Lightning
> var JointBPath : CogPath


---  
 #  Ratio : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The ratio between the two stick joints. The ratio is used in the formula "length0 + ratio * length1 = 0".
> ``` lang=cpp, name=Lightning
> var Ratio : Real


---  
 #  Methods


---  
 #  PulleyJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PulleyJoint()
> ``` 


---  
 

 
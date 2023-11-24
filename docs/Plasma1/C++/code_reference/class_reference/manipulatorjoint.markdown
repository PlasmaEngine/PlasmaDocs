 `Component` `Physics`



(NOTE) Legacy. A position joint that is designed to manipulate one object. The only difference between this and the position joint is that the manipulator always draws itself, draws differently, and configures the max impulse differently.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjoint.markdown#manipulatorjoint-void)|[ LocalPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjoint.markdown#localpoint-plasma-engine-d)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.markdown)| |
| |[ TargetPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjoint.markdown#targetpoint-plasma-engine)| | |
| |[ WorldPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjoint.markdown#worldpoint-plasma-engine-d)| | |


 #  Properties


---  
 #  LocalPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The local space point on the object that the joint is connected to.
> ``` lang=cpp, name=Lightning
> var LocalPoint : Real3


---  
 #  TargetPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The point in world space that the object's point is being moved towards.
> ``` lang=cpp, name=Lightning
> var TargetPoint : Real3


---  
 #  WorldPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The world space point on the object that the joint is connected to.
> ``` lang=cpp, name=Lightning
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  ManipulatorJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ManipulatorJoint()
> ``` 


---  
 

 
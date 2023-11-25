 `Component` `Physics`



(NOTE) Allows the user to override parameters for debug drawing of joints. Primarily used to debug draw from different object perspectives and to change the size of drawn data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#jointdebugdrawconfig-voi)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ Detail](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#detail-plasma-engine-docum)| | |
| |[ ObjectAPerspective](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#objectaperspective-plasma)| | |
| |[ ObjectBPerspective](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#objectbperspective-plasma)| | |
| |[ Size](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md#size-plasma-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not this component is active.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  Detail : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The amount of detail to use when drawing. For example, the detail on a RevoluteJoint will increase the number of lines used to draw the arc of a circle.
> ``` lang=cpp, name=Lightning
> var Detail : Real


---  
 #  ObjectAPerspective : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectA. Typically used when ObjectA is marked as a static object and ObjectB has free movement.
> ``` lang=cpp, name=Lightning
> var ObjectAPerspective : Boolean


---  
 #  ObjectBPerspective : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectB. Typically used when ObjectB is marked as a static object and ObjectA has free movement.
> ``` lang=cpp, name=Lightning
> var ObjectBPerspective : Boolean


---  
 #  Size : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> A size modifier for the debug drawing. 1 is the base size.
> ``` lang=cpp, name=Lightning
> var Size : Real


---  
 #  Methods


---  
 #  JointDebugDrawConfig : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function JointDebugDrawConfig()
> ``` 


---  
 

 
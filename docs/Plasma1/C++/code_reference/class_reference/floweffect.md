 `Component` `Physics`



(NOTE) Applies a force to make an object move at a target speed in a given direction. This can also be used to pull the object towards the center of the flow (the axis in the flow direction centered at the effect). Used to model a river or a tractor beam.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#floweffect-void)|[ AttractSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#attractspeed-plasma-engine)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)| |
| |[ AttractToFlowCenter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#attracttoflowcenter-plasma)| | |
| |[ FlowDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#flowdirection-plasma-engin)| | |
| |[ FlowSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#flowspeed-plasma-engine-do)| | |
| |[ LocalForce](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#localforce-plasma-engine-d)| | |
| |[ MaxAttractForce](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#maxattractforce-plasma-eng)| | |
| |[ MaxFlowForce](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#maxflowforce-plasma-engine)| | |
| |[ WorldFlowDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md#worldflowdirection-plasma)| | |


 #  Properties


---  
 #  AttractSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The target speed for an object to be pulled towards the center of the flow.
> ``` lang=cpp, name=Lightning
> var AttractSpeed : Real


---  
 #  AttractToFlowCenter : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the flow field will attract objects towards the center of the field. This can be used to create a tractor beam effect that will keep the object inside of the flow field.
> ``` lang=cpp, name=Lightning
> var AttractToFlowCenter : Boolean


---  
 #  FlowDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The direction that the field is flowing. This can be defined in world or local space.
> ``` lang=cpp, name=Lightning
> var FlowDirection : Real3


---  
 #  FlowSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The target speed of objects in the flow field.
> ``` lang=cpp, name=Lightning
> var FlowSpeed : Real


---  
 #  LocalForce : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the flow direction is in the local space of the object.
> ``` lang=cpp, name=Lightning
> var LocalForce : Boolean


---  
 #  MaxAttractForce : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max force that can be used to reach the target attract speed.
> ``` lang=cpp, name=Lightning
> var MaxAttractForce : Real


---  
 #  MaxFlowForce : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max force that can be used to reach the target flow speed.
> ``` lang=cpp, name=Lightning
> var MaxFlowForce : Real


---  
 #  WorldFlowDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The direction that the field is flowing in world space.
> ``` lang=cpp, name=Lightning
> var WorldFlowDirection : Real3


---  
 #  Methods


---  
 #  FlowEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FlowEffect()
> ``` 


---  
 

 
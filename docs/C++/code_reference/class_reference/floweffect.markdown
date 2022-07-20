 `Component` `Physics`



(NOTE) Applies a force to make an object move at a target speed in a given direction. This can also be used to pull the object towards the center of the flow (the axis in the flow direction centered at the effect). Used to model a river or a tractor beam.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#floweffect-void)|[ AttractSpeed](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#attractspeed-plasma-engine)|[physicseffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/physicseffect.markdown)| |
| |[ AttractToFlowCenter](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#attracttoflowcenter-plasma)| | |
| |[ FlowDirection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#flowdirection-plasma-engin)| | |
| |[ FlowSpeed](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#flowspeed-plasma-engine-do)| | |
| |[ LocalForce](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#localforce-plasma-engine-d)| | |
| |[ MaxAttractForce](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#maxattractforce-plasma-eng)| | |
| |[ MaxFlowForce](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#maxflowforce-plasma-engine)| | |
| |[ WorldFlowDirection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown#worldflowdirection-plasma)| | |


 #  Properties


---  
 #  AttractSpeed : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The target speed for an object to be pulled towards the center of the flow.
> ``` lang=cpp, name=Lightning
> var AttractSpeed : Real


---  
 #  AttractToFlowCenter : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Determines if the flow field will attract objects towards the center of the field. This can be used to create a tractor beam effect that will keep the object inside of the flow field.
> ``` lang=cpp, name=Lightning
> var AttractToFlowCenter : Boolean


---  
 #  FlowDirection : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The direction that the field is flowing. This can be defined in world or local space.
> ``` lang=cpp, name=Lightning
> var FlowDirection : Real3


---  
 #  FlowSpeed : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The target speed of objects in the flow field.
> ``` lang=cpp, name=Lightning
> var FlowSpeed : Real


---  
 #  LocalForce : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Determines if the flow direction is in the local space of the object.
> ``` lang=cpp, name=Lightning
> var LocalForce : Boolean


---  
 #  MaxAttractForce : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The max force that can be used to reach the target attract speed.
> ``` lang=cpp, name=Lightning
> var MaxAttractForce : Real


---  
 #  MaxFlowForce : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The max force that can be used to reach the target flow speed.
> ``` lang=cpp, name=Lightning
> var MaxFlowForce : Real


---  
 #  WorldFlowDirection : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

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
 

 
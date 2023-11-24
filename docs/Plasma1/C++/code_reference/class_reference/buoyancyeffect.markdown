 `Component` `Physics`



(NOTE) Applies a buoyancy force to an object in a given direction.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown#buoyancyeffect-void)|[ DebugDrawRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown#debugdrawruntime-plasma-en)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown)| |
| |[ Density](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown#density-plasma-engine-docu)| | |
| |[ Detail](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown#detail-plasma-engine-docum)| | |
| |[ Gravity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown#gravity-plasma-engine-docu)| | |


 #  Properties


---  
 #  DebugDrawRuntime : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Draw the points used to compute the buoyancy during run-time. This helps in debugging, but should be left off during normal run.
> ``` lang=cpp, name=Lightning
> var DebugDrawRuntime : Boolean


---  
 #  Density : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The density of the fluid.
> ``` lang=cpp, name=Lightning
> var Density : Real


---  
 #  Detail : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The amount of points to subdivide each object into for sampling (total points is Detail^3)
> ``` lang=cpp, name=Lightning
> var Detail : Integer


---  
 #  Gravity : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The direction of gravity in world-space.
> ``` lang=cpp, name=Lightning
> var Gravity : Real3


---  
 #  Methods


---  
 #  BuoyancyEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function BuoyancyEffect()
> ``` 


---  
 

 
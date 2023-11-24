 `Component` `Physics`



(NOTE) Applies a wind force in a given direction. The wind force is calculated from the squared wind speed and is scaled by the approximate surface area of the object in the direction of the force.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown#windeffect-void)|[ LocalSpaceDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown#localspacedirection-plasma)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown)| |
| |[ WindDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown#winddirection-plasma-engin)| | |
| |[ WindSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown#windspeed-plasma-engine-do)| | |
| |[ WorldWindDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown#worldwinddirection-plasma)| | |


 #  Properties


---  
 #  LocalSpaceDirection : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Determines if the wind's direction is a local or world-space vector.
> ``` lang=cpp, name=Lightning
> var LocalSpaceDirection : Boolean


---  
 #  WindDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The direction that the wind is blowing.
> ``` lang=cpp, name=Lightning
> var WindDirection : Real3


---  
 #  WindSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The speed that the wind is blowing.
> ``` lang=cpp, name=Lightning
> var WindSpeed : Real


---  
 #  WorldWindDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The direction of the wind in world space.
> ``` lang=cpp, name=Lightning
> var WorldWindDirection : Real3


---  
 #  Methods


---  
 #  WindEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WindEffect()
> ``` 


---  
 

 
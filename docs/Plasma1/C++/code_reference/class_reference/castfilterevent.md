 `Event` `Physics`



(NOTE) Allows a user to filter out an object during any cast in physics.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FilterState](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilterevent.md#filterstate-plasma-engine)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ Object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilterevent.md#object-plasma-engine-docum)| | |


 #  Properties


---  
 #  FilterState : [CastFilterState](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#castfilterstate)

> When filtering should we accept or reject this cog? Alternatively we can let the default cast filter logic run.
> ``` lang=cpp, name=Lightning
> var FilterState : CastFilterState


---  
 #  Object : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The object being tested in this cast.
> ``` lang=cpp, name=Lightning
> var Object : Cog


---  
 #  Methods


---  
 

 
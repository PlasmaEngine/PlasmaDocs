 `Component` `Physics`



(NOTE) Defines collision for a height map.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearCachedEdgeAdjacency](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md#clearcachededgeadjacency)|[ Thickness](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md#thickness-plasma-engine-do)|[collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md#heightmapcollider-void)| | | |


 #  Properties


---  
 #  Thickness : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How thick the surface of the height map is. Used to avoid tunneling problems.
> ``` lang=cpp, name=Lightning
> var Thickness : Real


---  
 #  Methods


---  
 #  ClearCachedEdgeAdjacency : Void

> Clear the cached information used to avoid catching edges. Typically called internally by physics, but is exposed for manual triggering.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearCachedEdgeAdjacency()
> ``` 


---  
 #  HeightMapCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function HeightMapCollider()
> ``` 


---  
 

 
 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#debugcapsule-void)|[ Color](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#color-plasma-engine-docume)| | |
| |[ End](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#end-plasma-engine-document)| | |
| |[ OnTop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#ontop-plasma-engine-docume)| | |
| |[ Radius](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#radius-plasma-engine-docum)| | |
| |[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#start-plasma-engine-docume)| | |
| |[ ViewAligned](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugcapsule.md#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  End : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var End : Real3


---  
 #  OnTop : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


---  
 #  Radius : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> 
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  Start : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Start : Real3


---  
 #  ViewAligned : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaleOffset : Real3


---  
 #  Methods


---  
 #  DebugCapsule : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugCapsule()
> ``` 


---  
 #  DebugCapsule : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |end|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |radius|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function DebugCapsule(start : Real3, end : Real3, radius : Real)
> ``` 


---  
 #  DebugCapsule : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |axis|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |height|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |radius|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function DebugCapsule(position : Real3, axis : Real3, height : Real, radius : Real)
> ``` 


---  
 

 
 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#debugline-void)|[ BoxHeads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#boxheads-plasma-engine-doc)| | |
| |[ Color](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#color-plasma-engine-docume)| | |
| |[ DualHeads](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#dualheads-plasma-engine-do)| | |
| |[ End](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#end-plasma-engine-document)| | |
| |[ Filled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#filled-plasma-engine-docum)| | |
| |[ HeadSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#headsize-plasma-engine-doc)| | |
| |[ OnTop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#ontop-plasma-engine-docume)| | |
| |[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#start-plasma-engine-docume)| | |
| |[ ViewAligned](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugline.md#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  BoxHeads : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var BoxHeads : Boolean


---  
 #  Color : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  DualHeads : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var DualHeads : Boolean


---  
 #  End : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var End : Real3


---  
 #  Filled : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var Filled : Boolean


---  
 #  HeadSize : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> 
> ``` lang=cpp, name=Lightning
> var HeadSize : Real


---  
 #  OnTop : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


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
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugLine()
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |ray|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(ray : Ray)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |ray|[ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)| |
> |t|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(ray : Ray, t : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |end|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(start : Real3, end : Real3)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |end|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |headSize|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(start : Real3, end : Real3, headSize : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(segment : Segment)
> ``` 


---  
 

 
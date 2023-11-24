 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#debugline-void)|[ BoxHeads](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#boxheads-plasma-engine-doc)| | |
| |[ Color](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#color-plasma-engine-docume)| | |
| |[ DualHeads](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#dualheads-plasma-engine-do)| | |
| |[ End](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#end-plasma-engine-document)| | |
| |[ Filled](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#filled-plasma-engine-docum)| | |
| |[ HeadSize](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#headsize-plasma-engine-doc)| | |
| |[ OnTop](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#ontop-plasma-engine-docume)| | |
| |[ Start](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#start-plasma-engine-docume)| | |
| |[ ViewAligned](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/debugline.markdown#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  BoxHeads : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var BoxHeads : Boolean


---  
 #  Color : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  DualHeads : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var DualHeads : Boolean


---  
 #  End : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var End : Real3


---  
 #  Filled : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Filled : Boolean


---  
 #  HeadSize : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HeadSize : Real


---  
 #  OnTop : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


---  
 #  Start : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Start : Real3


---  
 #  ViewAligned : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

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
> |ray|[ray](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ray.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(ray : Ray)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |ray|[ray](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/ray.markdown)| |
> |t|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(ray : Ray, t : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |end|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(start : Real3, end : Real3)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |end|[real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)| |
> |headSize|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(start : Real3, end : Real3, headSize : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/segment.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugLine(segment : Segment)
> ``` 


---  
 

 
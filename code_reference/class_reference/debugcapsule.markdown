 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#debugcapsule-void)|[ Color](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#color-plasma-engine-docume)| | |
| |[ End](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#end-plasma-engine-document)| | |
| |[ OnTop](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#ontop-plasma-engine-docume)| | |
| |[ Radius](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#radius-plasma-engine-docum)| | |
| |[ Start](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#start-plasma-engine-docume)| | |
| |[ ViewAligned](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/debugcapsule.markdown#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  End : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var End : Real3


---  
 #  OnTop : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


---  
 #  Radius : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Radius : Real


---  
 #  Start : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Start : Real3


---  
 #  ViewAligned : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

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
> |start|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |end|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |radius|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugCapsule(start : Real3, end : Real3, radius : Real)
> ``` 


---  
 #  DebugCapsule : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |axis|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |height|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |radius|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugCapsule(position : Real3, axis : Real3, height : Real, radius : Real)
> ``` 


---  
 

 
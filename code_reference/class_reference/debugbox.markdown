 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#debugbox-void)|[ Color](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#color-plasma-engine-docume)| | |
| |[ Filled](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#filled-plasma-engine-docum)| | |
| |[ HalfExtents](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#halfextents-plasma-engine)| | |
| |[ OnTop](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#ontop-plasma-engine-docume)| | |
| |[ Position](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#position-plasma-engine-doc)| | |
| |[ Rotation](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#rotation-plasma-engine-doc)| | |
| |[ ViewAligned](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/debugbox.markdown#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  Filled : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Filled : Boolean


---  
 #  HalfExtents : [real2](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HalfExtents : Real2


---  
 #  OnTop : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


---  
 #  Position : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Position : Real3


---  
 #  Rotation : [quaternion](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Rotation : Quaternion


---  
 #  ViewAligned : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaleOffset : Real3


---  
 #  Methods


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugBox()
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(aabb : Aabb)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |rotation|[quaternion](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real, rotation : Quaternion)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real2](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real2)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real2](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> |rotation|[quaternion](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real2, rotation : Quaternion)
> ``` 


---  
 

 
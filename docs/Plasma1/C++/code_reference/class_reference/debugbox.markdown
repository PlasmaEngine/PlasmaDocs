 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#debugbox-void)|[ Color](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#color-plasma-engine-docume)| | |
| |[ Filled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#filled-plasma-engine-docum)| | |
| |[ HalfExtents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#halfextents-plasma-engine)| | |
| |[ OnTop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#ontop-plasma-engine-docume)| | |
| |[ Position](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#position-plasma-engine-doc)| | |
| |[ Rotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#rotation-plasma-engine-doc)| | |
| |[ ViewAligned](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#viewaligned-plasma-engine)| | |
| |[ ViewScaled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#viewscaled-plasma-engine-d)| | |
| |[ ViewScaleOffset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/debugbox.markdown#viewscaleoffset-plasma-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  Filled : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Filled : Boolean


---  
 #  HalfExtents : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HalfExtents : Real2


---  
 #  OnTop : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var OnTop : Boolean


---  
 #  Position : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Position : Real3


---  
 #  Rotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Rotation : Quaternion


---  
 #  ViewAligned : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

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
> |aabb|[aabb](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/aabb.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(aabb : Aabb)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |rotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real, rotation : Quaternion)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real2)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |halfExtents|[real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)| |
> |rotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function DebugBox(position : Real3, halfExtents : Real2, rotation : Quaternion)
> ``` 


---  
 

 
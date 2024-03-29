 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md#getpoint-plasma-engine-doc)|[ End](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md#end-plasma-engine-document)| | |
|[ GetTValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md#gettvalue-plasma-engine-do)|[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md#start-plasma-engine-docume)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md#segment-void)| | | |


 #  Properties


---  
 #  End : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var End : Real3


---  
 #  Start : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> 
> ``` lang=cpp, name=Lightning
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Returns the t-value that would result in the given point projected onto the segment.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetTValue(point : Real3) : Real
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Segment()
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |end|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Segment(start : Real3, end : Real3)
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[segment](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/segment.md)| |
> ``` lang=cpp, name=Lightning
> function Segment(p0 : Segment)
> ``` 


---  
 

 
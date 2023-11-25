 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md#plane-void)|[ Data](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md#data-plasma-engine-documen)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md#set-void)|[ Distance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md#distance-plasma-engine-doc)| | |
| |[ Normal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md#normal-plasma-engine-docum)| | |


 #  Properties


---  
 #  Data : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var Data : Real4


---  
 #  Distance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Distance : Real


---  
 #  Normal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Normal : Real3


---  
 #  Methods


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Plane()
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[plane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plane.md)| |
> ``` lang=cpp, name=Lightning
> function Plane(p0 : Plane)
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Plane(normal : Real3, point : Real3)
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |data|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function Plane(data : Real4)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function Set(normal : Real3, point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |data|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function Set(data : Real4)
> ``` 


---  
 

 
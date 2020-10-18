 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown#getpoint-plasma-engine-doc)|[ Direction](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown#direction-plasma-engine-do)| | |
|[ GetTValue](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown#gettvalue-plasma-engine-do)|[ Start](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown#start-plasma-engine-docume)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown#ray-void)| | | |


 #  Properties


---  
 #  Direction : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Direction : Real3


---  
 #  Start : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Returns the t-value that would result in the given point projected onto the ray.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetTValue(point : Real3) : Real
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Ray()
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ray](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown)| |
> ``` lang=cpp, name=Lightning
> function Ray(p0 : Ray)
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |direction|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Ray(start : Real3, direction : Real3)
> ``` 


---  
 

 
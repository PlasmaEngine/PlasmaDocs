 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#boolean3-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#count-plasma-engine-docume)| | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#get-plasma-engine-document)|[ One](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#one-plasma-engine-document)| | |
|[ GetAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#getaxis-plasma-engine-docu)|[ XAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#xaxis-plasma-engine-docume)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#set-void)|[ YAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#yaxis-plasma-engine-docume)| | |
| |[ ZAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#zaxis-plasma-engine-docume)| | |
| |[ Zero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown#plasma-plasma-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  One : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Lightning
> var One : Boolean3


---  
 #  XAxis : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var XAxis : Boolean3


---  
 #  YAxis : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var YAxis : Boolean3


---  
 #  ZAxis : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var ZAxis : Boolean3


---  
 #  Zero : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `read-only` `static`

> The zero vector (a vector containing all plasmaes).
> ``` lang=cpp, name=Lightning
> var Zero : Boolean3


---  
 #  Methods


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Boolean3()
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Boolean3(scalar : Boolean)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> |p1|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> |p2|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Boolean3(p0 : Boolean, p1 : Boolean, p2 : Boolean)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> |p1|[boolean2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean2.markdown)| |
> ``` lang=cpp, name=Lightning
> function Boolean3(p0 : Boolean, p1 : Boolean2)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean2.markdown)| |
> |p1|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Boolean3(p0 : Boolean2, p1 : Boolean)
> ``` 


---  
 #  Get : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(p0 : Integer) : Boolean
> ``` 


---  
 #  GetAxis : [boolean3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean3.markdown)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxis(p0 : Integer) : Boolean3
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |p1|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(p0 : Integer, p1 : Boolean)
> ``` 


---  
 

 
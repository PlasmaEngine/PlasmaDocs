 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#boolean-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#count-plasma-engine-docume)| | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#get-plasma-engine-document)|[ One](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#one-plasma-engine-document)| | |
|[ GetAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#getaxis-plasma-engine-docu)|[ XAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#xaxis-plasma-engine-docume)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#set-void)|[ Zero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown#plasma-plasma-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  One : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Lightning
> var One : Boolean


---  
 #  XAxis : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var XAxis : Boolean


---  
 #  Zero : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only` `static`

> The zero vector (a vector containing all plasmaes).
> ``` lang=cpp, name=Lightning
> var Zero : Boolean


---  
 #  Methods


---  
 #  Boolean : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Boolean()
> ``` 


---  
 #  Boolean : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function Boolean(scalar : Boolean)
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
 #  GetAxis : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxis(p0 : Integer) : Boolean
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
 

 
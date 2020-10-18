 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#get-plasma-engine-document)|[ Count](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#count-plasma-engine-docume)| | |
|[ GetByIndex](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#getbyindex-plasma-engine-d)|[ CountX](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#countx-plasma-engine-docum)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#real2x3-void)|[ CountY](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#county-plasma-engine-docum)| | |
|[ Set](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#set-void)|[ M00](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m00-plasma-engine-document)| | |
|[ SetByIndex](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#setbyindex-void)|[ M01](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m01-plasma-engine-document)| | |
| |[ M02](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m02-plasma-engine-document)| | |
| |[ M10](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m10-plasma-engine-document)| | |
| |[ M11](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m11-plasma-engine-document)| | |
| |[ M12](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2x3.markdown#m12-plasma-engine-document)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  CountX : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CountX : Integer


---  
 #  CountY : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CountY : Integer


---  
 #  M00 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M00 : Real


---  
 #  M01 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M01 : Real


---  
 #  M02 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M02 : Real


---  
 #  M10 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M10 : Real


---  
 #  M11 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M11 : Real


---  
 #  M12 : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var M12 : Real


---  
 #  Methods


---  
 #  Get : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(y : Integer) : Real3
> ``` 


---  
 #  Get : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |x|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(y : Integer, x : Integer) : Real
> ``` 


---  
 #  GetByIndex : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetByIndex(index : Integer) : Real
> ``` 


---  
 #  Real2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Real2x3()
> ``` 


---  
 #  Real2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2x3(p0 : Real)
> ``` 


---  
 #  Real2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |m01|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |m02|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |m10|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |m11|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |m12|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2x3(m00 : Real, m01 : Real, m02 : Real, m10 : Real, m11 : Real, m12 : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |x|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |value|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(y : Integer, x : Integer, value : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |value|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(y : Integer, value : Real3)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |value|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetByIndex(index : Integer, value : Real)
> ``` 


---  
 

 
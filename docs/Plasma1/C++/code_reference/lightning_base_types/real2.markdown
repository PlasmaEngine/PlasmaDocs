 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#get-plasma-engine-document)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#count-plasma-engine-docume)| | |
|[ GetAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#getaxis-plasma-engine-docu)|[ NegativeMin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#negativemin-plasma-engine)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#real2-void)|[ NegativeValueClosestToZero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#negativevalueclosesttoze)| | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#set-void)|[ One](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#one-plasma-engine-document)| | |
| |[ PositiveMax](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#positivemax-plasma-engine)| | |
| |[ PositiveValueClosestToZero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#positivevalueclosesttoze)| | |
| |[ XAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#xaxis-plasma-engine-docume)| | |
| |[ YAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#yaxis-plasma-engine-docume)| | |
| |[ Zero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown#plasma-plasma-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  NegativeMin : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ``` lang=cpp, name=Lightning
> var NegativeMin : Real2


---  
 #  NegativeValueClosestToZero : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Lightning
> var NegativeValueClosestToZero : Real2


---  
 #  One : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Lightning
> var One : Real2


---  
 #  PositiveMax : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ``` lang=cpp, name=Lightning
> var PositiveMax : Real2


---  
 #  PositiveValueClosestToZero : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Lightning
> var PositiveValueClosestToZero : Real2


---  
 #  XAxis : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var XAxis : Real2


---  
 #  YAxis : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var YAxis : Real2


---  
 #  Zero : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `read-only` `static`

> The zero vector (a vector containing all plasmaes).
> ``` lang=cpp, name=Lightning
> var Zero : Real2


---  
 #  Methods


---  
 #  Get : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(p0 : Integer) : Real
> ``` 


---  
 #  GetAxis : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxis(p0 : Integer) : Real2
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Real2()
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2(scalar : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |p1|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2(p0 : Real, p1 : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2(p0 : Real2)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |p1|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(p0 : Integer, p1 : Real)
> ``` 


---  
 

 
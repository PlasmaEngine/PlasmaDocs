 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md#parse-plasma-engine-docume)|[ NegativeMin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md#negativemin-plasma-engine)| | |
| |[ NegativeValueClosestToZero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md#negativevalueclosesttoze)| | |
| |[ PositiveMax](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md#positivemax-plasma-engine)| | |
| |[ PositiveValueClosestToZero](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  NegativeMin : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a DoubleReal.
> ``` lang=cpp, name=Lightning
> var NegativeMin : DoubleReal


---  
 #  NegativeValueClosestToZero : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a DoubleReal.
> ``` lang=cpp, name=Lightning
> var NegativeValueClosestToZero : DoubleReal


---  
 #  PositiveMax : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a DoubleReal.
> ``` lang=cpp, name=Lightning
> var PositiveMax : DoubleReal


---  
 #  PositiveValueClosestToZero : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a DoubleReal.
> ``` lang=cpp, name=Lightning
> var PositiveValueClosestToZero : DoubleReal


---  
 #  Methods


---  
 #  Parse : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.md)

 `static`

> Attempt to convert the given StringRange to a DoubleReal. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/stringrange.md)| |
> ``` lang=cpp, name=Lightning
> function Parse(p0 : StringRange) : DoubleReal
> ``` 


---  
 

 
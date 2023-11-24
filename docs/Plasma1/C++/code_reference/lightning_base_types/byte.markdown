 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown#parse-plasma-engine-docume)|[ PositiveMax](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown#positivemax-plasma-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  PositiveMax : [byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Byte.
> ``` lang=cpp, name=Lightning
> var PositiveMax : Byte


---  
 #  PositiveValueClosestToZero : [byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Byte.
> ``` lang=cpp, name=Lightning
> var PositiveValueClosestToZero : Byte


---  
 #  Methods


---  
 #  Parse : [byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)

 `static`

> Attempt to convert the given StringRange to a Byte. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringrange.markdown)| |
> ``` lang=cpp, name=Lightning
> function Parse(p0 : StringRange) : Byte
> ``` 


---  
 

 
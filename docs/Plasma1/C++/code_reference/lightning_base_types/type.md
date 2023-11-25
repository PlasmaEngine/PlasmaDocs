 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isa-plasma-engine-document)|[ IsAny](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isany-plasma-engine-docume)|[reflectionobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/reflectionobject.md)|[anytype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anytype.md)|
|[ IsCastableTo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#iscastableto-plasma-engine)|[ IsDelegate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isdelegate-plasma-engine-d)| |[boundtype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boundtype.md)|
|[ IsRawCastableTo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#israwcastableto-plasma-eng)|[ IsEnum](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isenum-plasma-engine-docum)| |[delegatetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/delegatetype.md)|
| |[ IsEnumOrFlags](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isenumorflags-plasma-engin)| |[indirectiontype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/indirectiontype.md)|
| |[ IsFlags](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isflags-plasma-engine-docu)| | |
| |[ IsHandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#ishandle-plasma-engine-doc)| | |
| |[ IsValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#isvalue-plasma-engine-docu)| | |
| |[ Library](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#library-plasma-engine-docu)| | |
| |[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md#name-plasma-engine-documen)| | |


 #  Properties


---  
 #  IsAny : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsAny : Boolean


---  
 #  IsDelegate : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsDelegate : Boolean


---  
 #  IsEnum : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsEnum : Boolean


---  
 #  IsEnumOrFlags : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsEnumOrFlags : Boolean


---  
 #  IsFlags : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsFlags : Boolean


---  
 #  IsHandle : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsHandle : Boolean


---  
 #  IsValue : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var IsValue : Boolean


---  
 #  Library : [library](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/library.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Library : Library


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Methods


---  
 #  IsA : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |baseType|[type](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md)| |
> ``` lang=cpp, name=Lightning
> function IsA(baseType : Type) : Boolean
> ``` 


---  
 #  IsCastableTo : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md)| |
> ``` lang=cpp, name=Lightning
> function IsCastableTo(toType : Type) : Boolean
> ``` 


---  
 #  IsRawCastableTo : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/type.md)| |
> ``` lang=cpp, name=Lightning
> function IsRawCastableTo(toType : Type) : Boolean
> ``` 


---  
 

 
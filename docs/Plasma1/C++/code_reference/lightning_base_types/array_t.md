 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#add-void)|[ All](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#all-plasma-engine-document)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#array-t-void)|[ Capacity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#capacity-plasma-engine-doc)| | |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#clear-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#count-plasma-engine-docume)| | |
|[ Copy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#copy-plasma-engine-documen)|[ LastIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#lastindex-plasma-engine-do)| | |
|[ FindFirstIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#findfirstindex-plasma-engi)| | | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#get-plasma-engine-document)| | | |
|[ Insert](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#insert-void)| | | |
|[ Pop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#pop-plasma-engine-document)| | | |
|[ Push](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#push-void)| | | |
|[ Range](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#range-plasma-engine-docume)| | | |
|[ RemoveAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#removeall-plasma-engine-do)| | | |
|[ RemoveAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#removeat-void)| | | |
|[ RemoveFirst](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#removefirst-plasma-engine)| | | |
|[ RemoveSwap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#removeswap-void)| | | |
|[ Reserve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#reserve-void)| | | |
|[ Resize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#resize-void)| | | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#set-void)| | | |
|[ Sort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t .md#sort-void)| | | |


 #  Properties


---  
 #  All : ArrayRange[T]

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var All : ArrayRange[T]


---  
 #  Capacity : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Capacity : Integer


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  LastIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var LastIndex : Integer


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ``` lang=cpp, name=Lightning
> function Add(p0 : T)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Array[T]()
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Array[T](size : Integer)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |defaultValue|T| |
> ``` lang=cpp, name=Lightning
> function Array[T](size : Integer, defaultValue : T)
> ``` 


---  
 #  Clear : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Copy : Array[T]

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Copy() : Array[T]
> ``` 


---  
 #  FindFirstIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Lightning
> function FindFirstIndex(value : T) : Integer
> ``` 


---  
 #  Get : T

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : T
> ``` 


---  
 #  Insert : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |value|T| |
> ``` lang=cpp, name=Lightning
> function Insert(index : Integer, value : T)
> ``` 


---  
 #  Pop : T

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Pop() : T
> ``` 


---  
 #  Push : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ``` lang=cpp, name=Lightning
> function Push(p0 : T)
> ``` 


---  
 #  Range : ArrayRange[T]

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |count|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Range(start : Integer, count : Integer) : ArrayRange[T]
> ``` 


---  
 #  RemoveAll : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Lightning
> function RemoveAll(value : T) : Integer
> ``` 


---  
 #  RemoveAt : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveFirst : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Lightning
> function RemoveFirst(value : T) : Boolean
> ``` 


---  
 #  RemoveSwap : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveSwap(index : Integer)
> ``` 


---  
 #  Reserve : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |capacity|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Reserve(capacity : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Resize(size : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |defaultValue|T| |
> ``` lang=cpp, name=Lightning
> function Resize(size : Integer, defaultValue : T)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |value|T| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, value : T)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function Sort(compare : delegate(left:any,right:any):Boolean)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Sort(compare : delegate(left:any,right:any):Integer)
> ``` 


---  
 

 
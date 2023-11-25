 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md#iencoding-void)|[ Ascii](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md#ascii-plasma-engine-docume)| |[asciiencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/asciiencoding.md)|
|[ Read](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md#read-plasma-engine-documen)|[ Utf8](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md#utf8-plasma-engine-documen)| |[utf8encoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/utf8encoding.md)|
|[ Write](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md#write-plasma-engine-docume)| | | |


 #  Properties


---  
 #  Ascii : [asciiencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/asciiencoding.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Ascii : AsciiEncoding


---  
 #  Utf8 : [utf8encoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/utf8encoding.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Utf8 : Utf8Encoding


---  
 #  Methods


---  
 #  IEncoding : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IEncoding()
> ``` 


---  
 #  Read : [rune](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/rune.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[istream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md)| |
> ``` lang=cpp, name=Lightning
> function Read(p0 : IStream) : Rune
> ``` 


---  
 #  Write : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/rune.md)| |
> |p1|[istream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md)| |
> ``` lang=cpp, name=Lightning
> function Write(p0 : Rune, p1 : IStream) : Integer
> ``` 


---  
 

 
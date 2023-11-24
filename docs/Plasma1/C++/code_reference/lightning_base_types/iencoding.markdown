 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.markdown#iencoding-void)|[ Ascii](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.markdown#ascii-plasma-engine-docume)| |[asciiencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/asciiencoding.markdown)|
|[ Read](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.markdown#read-plasma-engine-documen)|[ Utf8](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.markdown#utf8-plasma-engine-documen)| |[utf8encoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/utf8encoding.markdown)|
|[ Write](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.markdown#write-plasma-engine-docume)| | | |


 #  Properties


---  
 #  Ascii : [asciiencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/asciiencoding.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Ascii : AsciiEncoding


---  
 #  Utf8 : [utf8encoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/utf8encoding.markdown)

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
 #  Read : [rune](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/rune.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[istream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.markdown)| |
> ``` lang=cpp, name=Lightning
> function Read(p0 : IStream) : Rune
> ``` 


---  
 #  Write : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/rune.markdown)| |
> |p1|[istream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.markdown)| |
> ``` lang=cpp, name=Lightning
> function Write(p0 : Rune, p1 : IStream) : Integer
> ``` 


---  
 

 
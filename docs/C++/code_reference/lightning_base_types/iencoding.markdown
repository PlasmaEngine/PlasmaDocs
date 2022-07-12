 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/iencoding.markdown#iencoding-void)|[ Ascii](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/iencoding.markdown#ascii-plasma-engine-docume)| |[asciiencoding](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/asciiencoding.markdown)|
|[ Read](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/iencoding.markdown#read-plasma-engine-documen)|[ Utf8](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/iencoding.markdown#utf8-plasma-engine-documen)| |[utf8encoding](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/utf8encoding.markdown)|
|[ Write](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/iencoding.markdown#write-plasma-engine-docume)| | | |


 #  Properties


---  
 #  Ascii : [asciiencoding](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/asciiencoding.markdown)

 `read-only` `static`

> 
> ``` lang=cpp, name=Lightning
> var Ascii : AsciiEncoding


---  
 #  Utf8 : [utf8encoding](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/utf8encoding.markdown)

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
 #  Read : [rune](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/rune.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[istream](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/istream.markdown)| |
> ``` lang=cpp, name=Lightning
> function Read(p0 : IStream) : Rune
> ``` 


---  
 #  Write : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/rune.markdown)| |
> |p1|[istream](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/istream.markdown)| |
> ``` lang=cpp, name=Lightning
> function Write(p0 : Rune, p1 : IStream) : Integer
> ``` 


---  
 

 
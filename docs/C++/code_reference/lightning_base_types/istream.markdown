 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Flush](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#flush-void)|[ Capabilities](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#capabilities-plasma-engine)| |[filestream](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/filestream.markdown)|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#istream-void)|[ Count](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#count-plasma-engine-docume)| | |
|[ Read](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#read-plasma-engine-documen)|[ Position](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#position-plasma-engine-doc)| | |
|[ ReadAllText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#readalltext-plasma-engine)| | | |
|[ ReadByte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#readbyte-plasma-engine-doc)| | | |
|[ ReadLine](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#readline-plasma-engine-doc)| | | |
|[ Seek](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#seek-plasma-engine-documen)| | | |
|[ Write](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#write-plasma-engine-docume)| | | |
|[ WriteByte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#writebyte-plasma-engine-do)| | | |
|[ WriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/istream.markdown#writetext-plasma-engine-do)| | | |


 #  Properties


---  
 #  Capabilities : [StreamCapabilities](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/flags_reference.markdown#streamcapabilities)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Capabilities : StreamCapabilities


---  
 #  Count : [doubleinteger](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/doubleinteger.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Count : DoubleInteger


---  
 #  Position : [doubleinteger](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/doubleinteger.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Position : DoubleInteger


---  
 #  Methods


---  
 #  Flush : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Flush()
> ``` 


---  
 #  IStream : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IStream()
> ``` 


---  
 #  Read : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)]| |
> |byteStart|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |byteCount|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Read(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  ReadAllText : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadAllText() : String
> ``` 


---  
 #  ReadAllText : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/iencoding.markdown)| |
> ``` lang=cpp, name=Lightning
> function ReadAllText(p0 : IEncoding) : String
> ``` 


---  
 #  ReadByte : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadByte() : Integer
> ``` 


---  
 #  ReadLine : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadLine() : String
> ``` 


---  
 #  ReadLine : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/iencoding.markdown)| |
> ``` lang=cpp, name=Lightning
> function ReadLine(p0 : IEncoding) : String
> ``` 


---  
 #  Seek : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[doubleinteger](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/doubleinteger.markdown)| |
> |origin|[StreamOrigin](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#streamorigin)| |
> ``` lang=cpp, name=Lightning
> function Seek(position : DoubleInteger, origin : StreamOrigin) : Boolean
> ``` 


---  
 #  Write : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)]| |
> ``` lang=cpp, name=Lightning
> function Write(data : Array[Byte]) : Integer
> ``` 


---  
 #  Write : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)]| |
> |byteStart|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |byteCount|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Write(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  WriteByte : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[byte](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/byte.markdown)| |
> ``` lang=cpp, name=Lightning
> function WriteByte(p0 : Byte) : Integer
> ``` 


---  
 #  WriteText : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function WriteText(text : String) : Integer
> ``` 


---  
 #  WriteText : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> |sourceStreamEncoding|[iencoding](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/iencoding.markdown)| |
> ``` lang=cpp, name=Lightning
> function WriteText(text : String, sourceStreamEncoding : IEncoding) : Integer
> ``` 


---  
 

 
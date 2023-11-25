 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Flush](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#flush-void)|[ Capabilities](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#capabilities-plasma-engine)| |[filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.md)|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#istream-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#count-plasma-engine-docume)| | |
|[ Read](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#read-plasma-engine-documen)|[ Position](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#position-plasma-engine-doc)| | |
|[ ReadAllText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#readalltext-plasma-engine)| | | |
|[ ReadByte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#readbyte-plasma-engine-doc)| | | |
|[ ReadLine](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#readline-plasma-engine-doc)| | | |
|[ Seek](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#seek-plasma-engine-documen)| | | |
|[ Write](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#write-plasma-engine-docume)| | | |
|[ WriteByte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#writebyte-plasma-engine-do)| | | |
|[ WriteText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/istream.md#writetext-plasma-engine-do)| | | |


 #  Properties


---  
 #  Capabilities : [StreamCapabilities](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/flags_reference.md#streamcapabilities)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Capabilities : StreamCapabilities


---  
 #  Count : [doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.md)

> 
> ``` lang=cpp, name=Lightning
> var Count : DoubleInteger


---  
 #  Position : [doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.md)

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
 #  Read : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/byte.md)]| |
> |byteStart|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |byteCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Read(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  ReadAllText : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadAllText() : String
> ``` 


---  
 #  ReadAllText : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md)| |
> ``` lang=cpp, name=Lightning
> function ReadAllText(p0 : IEncoding) : String
> ``` 


---  
 #  ReadByte : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadByte() : Integer
> ``` 


---  
 #  ReadLine : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReadLine() : String
> ``` 


---  
 #  ReadLine : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md)| |
> ``` lang=cpp, name=Lightning
> function ReadLine(p0 : IEncoding) : String
> ``` 


---  
 #  Seek : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.md)| |
> |origin|[StreamOrigin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#streamorigin)| |
> ``` lang=cpp, name=Lightning
> function Seek(position : DoubleInteger, origin : StreamOrigin) : Boolean
> ``` 


---  
 #  Write : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/byte.md)]| |
> ``` lang=cpp, name=Lightning
> function Write(data : Array[Byte]) : Integer
> ``` 


---  
 #  Write : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/byte.md)]| |
> |byteStart|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |byteCount|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Write(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  WriteByte : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[byte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/byte.md)| |
> ``` lang=cpp, name=Lightning
> function WriteByte(p0 : Byte) : Integer
> ``` 


---  
 #  WriteText : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function WriteText(text : String) : Integer
> ``` 


---  
 #  WriteText : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |sourceStreamEncoding|[iencoding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/iencoding.md)| |
> ``` lang=cpp, name=Lightning
> function WriteText(text : String, sourceStreamEncoding : IEncoding) : Integer
> ``` 


---  
 

 
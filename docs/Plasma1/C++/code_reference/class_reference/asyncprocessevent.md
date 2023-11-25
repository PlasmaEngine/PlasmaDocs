 `Event` `Engine`



(NOTE) Sent out when AsyncProcess completes a partial read for a stream or the stream has finished reading all data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocessevent.md#asyncprocessevent-void)|[ Bytes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocessevent.md#bytes-plasma-engine-docume)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
| |[ StreamType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocessevent.md#streamtype-plasma-engine-d)| | |


 #  Properties


---  
 #  Bytes : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Bytes being read from a stream. Note: These bytes may not form a valid string if the stream type was non ascii (e.g. utf-8).
> ``` lang=cpp, name=Lightning
> var Bytes : String


---  
 #  StreamType : [StreamType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#streamtype)

> The type of stream that sent this event.
> ``` lang=cpp, name=Lightning
> var StreamType : StreamType


---  
 #  Methods


---  
 #  AsyncProcessEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AsyncProcessEvent()
> ``` 


---  
 

 
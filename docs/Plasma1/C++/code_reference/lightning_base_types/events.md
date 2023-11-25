 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/events.md#connect-void)| | | |
|[ Send](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/events.md#send-plasma-engine-documen)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Connect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |callback|delegate()| |
> ``` lang=cpp, name=Lightning
> function Connect(sender : AnyHandle, eventName : String, callback : delegate())
> ``` 


---  
 #  Send : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)| |
> |eventName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[eventdata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/eventdata.md)| |
> ``` lang=cpp, name=Lightning
> function Send(sender : AnyHandle, eventName : String, event : EventData) : Integer
> ``` 


---  
 

 
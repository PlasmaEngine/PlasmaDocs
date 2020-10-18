 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/events.markdown#connect-void)| | | |
|[ Send](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/events.markdown#send-plasma-engine-documen)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Connect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/anyhandle.markdown)| |
> |eventName|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |callback|delegate()| |
> ``` lang=cpp, name=Lightning
> function Connect(sender : AnyHandle, eventName : String, callback : delegate())
> ``` 


---  
 #  Send : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |sender|[anyhandle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/anyhandle.markdown)| |
> |eventName|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[eventdata](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/eventdata.markdown)| |
> ``` lang=cpp, name=Lightning
> function Send(sender : AnyHandle, eventName : String, event : EventData) : Integer
> ``` 


---  
 

 
 `Engine`

(NOTE) Keyboard representing the physical keyboard.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetKeyName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#getkeyname-plasma-engine-d)| |[eventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventobject.markdown)| |
|[ IsAnyKeyDown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#isanykeydown-plasma-engine)| | | |
|[ IsAnyNonModifierDown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#isanynonmodifierdown-zer)| | | |
|[ KeyIsDown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#keyisdown-plasma-engine-do)| | | |
|[ KeyIsPressed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#keyispressed-plasma-engine)| | | |
|[ KeyIsReleased](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#keyisreleased-plasma-engin)| | | |
|[ KeyIsUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#keyisup-plasma-engine-docu)| | | |
|[ ToKey](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#tokey-plasma-engine-docume)| | | |
|[ ToSymbol](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#tosymbol-plasma-engine-doc)| | | |
|[ Valid](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/keyboard.markdown#valid-plasma-engine-docume)| | | |


 #  Properties


---  
 #  Methods


---  
 #  GetKeyName : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> Gets a string name of a particular key.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function GetKeyName(key : Keys) : String
> ``` 


---  
 #  IsAnyKeyDown : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsAnyKeyDown() : Boolean
> ``` 


---  
 #  IsAnyNonModifierDown : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Excluding Ctrl, Shift, and Alt - is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsAnyNonModifierDown() : Boolean
> ``` 


---  
 #  KeyIsDown : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is the particular currently down.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsDown(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsPressed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Was the key pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsPressed(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsReleased : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Was the key released this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsReleased(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsUp : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Is the particular currently up.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsUp(key : Keys) : Boolean
> ``` 


---  
 #  ToKey : [Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)

> Counterpart to 'ToSymbol'. Converts a key's name or symbol to the key value. Returns Keys::Unknown if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function ToKey(key : String) : Keys
> ``` 


---  
 #  ToSymbol : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> Convert key value to it's actual name or keyboard symbol, if it has one. Returns "Unknown" String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function ToSymbol(key : Keys) : String
> ``` 


---  
 #  ToSymbol : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> Convert a key name to it's keyboard symbol, if it has one. Returns input String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |keyName|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function ToSymbol(keyName : String) : String
> ``` 


---  
 #  Valid : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Validate that the key is a Keys::Enum that is not 'Unknown', or 'None', or an integer value that doesn't map to a known Keys::Enum value.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#keys)| |
> ``` lang=cpp, name=Lightning
> function Valid(key : Keys) : Boolean
> ``` 


---  
 #  Valid : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Validate that the input string can be mapped back to an enum.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function Valid(key : String) : Boolean
> ``` 


---  
 

 
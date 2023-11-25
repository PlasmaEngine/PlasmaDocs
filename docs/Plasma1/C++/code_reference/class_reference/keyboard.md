 `Engine`

(NOTE) Keyboard representing the physical keyboard.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetKeyName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#getkeyname-plasma-engine-d)| |[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ IsAnyKeyDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#isanykeydown-plasma-engine)| | | |
|[ IsAnyNonModifierDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#isanynonmodifierdown-zer)| | | |
|[ KeyIsDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#keyisdown-plasma-engine-do)| | | |
|[ KeyIsPressed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#keyispressed-plasma-engine)| | | |
|[ KeyIsReleased](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#keyisreleased-plasma-engin)| | | |
|[ KeyIsUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#keyisup-plasma-engine-docu)| | | |
|[ ToKey](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#tokey-plasma-engine-docume)| | | |
|[ ToSymbol](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#tosymbol-plasma-engine-doc)| | | |
|[ Valid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#valid-plasma-engine-docume)| | | |


 #  Properties


---  
 #  Methods


---  
 #  GetKeyName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Gets a string name of a particular key.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function GetKeyName(key : Keys) : String
> ``` 


---  
 #  IsAnyKeyDown : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsAnyKeyDown() : Boolean
> ``` 


---  
 #  IsAnyNonModifierDown : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Excluding Ctrl, Shift, and Alt - is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsAnyNonModifierDown() : Boolean
> ``` 


---  
 #  KeyIsDown : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the particular currently down.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsDown(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsPressed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Was the key pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsPressed(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsReleased : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Was the key released this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsReleased(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsUp : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the particular currently up.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function KeyIsUp(key : Keys) : Boolean
> ``` 


---  
 #  ToKey : [Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)

> Counterpart to 'ToSymbol'. Converts a key's name or symbol to the key value. Returns Keys::Unknown if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function ToKey(key : String) : Keys
> ``` 


---  
 #  ToSymbol : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Convert key value to it's actual name or keyboard symbol, if it has one. Returns "Unknown" String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function ToSymbol(key : Keys) : String
> ``` 


---  
 #  ToSymbol : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Convert a key name to it's keyboard symbol, if it has one. Returns input String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |keyName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function ToSymbol(keyName : String) : String
> ``` 


---  
 #  Valid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Validate that the key is a Keys::Enum that is not 'Unknown', or 'None', or an integer value that doesn't map to a known Keys::Enum value.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Lightning
> function Valid(key : Keys) : Boolean
> ``` 


---  
 #  Valid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Validate that the input string can be mapped back to an enum.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function Valid(key : String) : Boolean
> ``` 


---  
 

 
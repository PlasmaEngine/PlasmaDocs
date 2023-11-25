 `Widget`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddCommandByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#addcommandbyname-plasma-en)|[ Icon](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#icon-plasma-engine-documen)|[safeid32eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32eventobject.md)|[contextmenuentrycommand](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentrycommand.md)|
|[ AddDivider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#adddivider-plasma-engine-d)|[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#name-plasma-engine-documen)| |[contextmenuentrydivider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentrydivider.md)|
|[ AddEntry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#addentry-plasma-engine-doc)| | |[contextmenuentrymenu](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentrymenu.md)|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#contextmenuentry-void)| | | |
|[ Entries](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#entries-plasma-engine-docu)| | | |
|[ GetEntry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#getentry-plasma-engine-doc)| | | |
|[ RemoveEntry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md#removeentry-void)| | | |


 #  Properties


---  
 #  Icon : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var Icon : String


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Methods


---  
 #  AddCommandByName : [contextmenuentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |commandName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function AddCommandByName(commandName : String) : ContextMenuEntry
> ``` 


---  
 #  AddDivider : [contextmenuentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AddDivider() : ContextMenuEntry
> ``` 


---  
 #  AddEntry : [contextmenuentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md)

> Adds a new entry with the provided name with an icon if one is provided to this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function AddEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  ContextMenuEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ContextMenuEntry()
> ``` 


---  
 #  Entries : [contextmenuentrychildrenrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentrychildrenrange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Entries() : ContextMenuEntryChildrenRange
> ``` 


---  
 #  GetEntry : [contextmenuentry](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contextmenuentry.md)

> Returns the children entry with the provided name if it exists and null otherwise.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  RemoveEntry : Void

> Remove the entry with the provided name from this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveEntry(name : String)
> ``` 


---  
 

 
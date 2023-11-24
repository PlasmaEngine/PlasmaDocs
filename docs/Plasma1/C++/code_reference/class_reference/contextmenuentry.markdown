 `Widget`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddCommandByName](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#addcommandbyname-plasma-en)|[ Icon](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#icon-plasma-engine-documen)|[safeid32eventobject](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/safeid32eventobject.markdown)|[contextmenuentrycommand](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentrycommand.markdown)|
|[ AddDivider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#adddivider-plasma-engine-d)|[ Name](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#name-plasma-engine-documen)| |[contextmenuentrydivider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentrydivider.markdown)|
|[ AddEntry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#addentry-plasma-engine-doc)| | |[contextmenuentrymenu](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentrymenu.markdown)|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#contextmenuentry-void)| | | |
|[ Entries](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#entries-plasma-engine-docu)| | | |
|[ GetEntry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#getentry-plasma-engine-doc)| | | |
|[ RemoveEntry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown#removeentry-void)| | | |


 #  Properties


---  
 #  Icon : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Icon : String


---  
 #  Name : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Methods


---  
 #  AddCommandByName : [contextmenuentry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |commandName|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddCommandByName(commandName : String) : ContextMenuEntry
> ``` 


---  
 #  AddDivider : [contextmenuentry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AddDivider() : ContextMenuEntry
> ``` 


---  
 #  AddEntry : [contextmenuentry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown)

> Adds a new entry with the provided name with an icon if one is provided to this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
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
 #  Entries : [contextmenuentrychildrenrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentrychildrenrange.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Entries() : ContextMenuEntryChildrenRange
> ``` 


---  
 #  GetEntry : [contextmenuentry](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contextmenuentry.markdown)

> Returns the children entry with the provided name if it exists and null otherwise.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  RemoveEntry : Void

> Remove the entry with the provided name from this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveEntry(name : String)
> ``` 


---  
 

 
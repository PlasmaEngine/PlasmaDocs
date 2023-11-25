 `Graphics`

(NOTE) Indexable interface for settings BlendSettings.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/blendsettingsmrt.md#get-plasma-engine-document)| |[threadsafereferencecounted](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/threadsafereferencecounted.md)| |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/blendsettingsmrt.md#set-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Get : [blendsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/blendsettings.md)

> Get the current BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : BlendSettings
> ``` 


---  
 #  Set : Void

> Set the BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |blendSettings|[blendsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/blendsettings.md)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, blendSettings : BlendSettings)
> ``` 


---  
 

 
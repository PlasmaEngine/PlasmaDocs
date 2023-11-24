 `Graphics`

(NOTE) Indexable interface for settings BlendSettings.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/blendsettingsmrt.markdown#get-plasma-engine-document)| |[threadsafereferencecounted](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/threadsafereferencecounted.markdown)| |
|[ Set](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/blendsettingsmrt.markdown#set-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Get : [blendsettings](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/blendsettings.markdown)

> Get the current BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : BlendSettings
> ``` 


---  
 #  Set : Void

> Set the BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> |blendSettings|[blendsettings](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/blendsettings.markdown)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, blendSettings : BlendSettings)
> ``` 


---  
 

 
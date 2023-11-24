 `Event` `Editor`



(NOTE) Allows Ui customization for Tools. This will be sent on the Tool every time it is activated.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ NeedsPropertyGrid](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/tooluievent.markdown#needspropertygrid-plasma-e)|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.markdown)| |
| |[ Parent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/tooluievent.markdown#parent-plasma-engine-docum)| | |
| |[ SelectTool](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/tooluievent.markdown#selecttool-plasma-engine-d)| | |


 #  Properties


---  
 #  NeedsPropertyGrid : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to force show the tools window when switched to this tool.
> ``` lang=cpp, name=Lightning
> var NeedsPropertyGrid : Boolean


---  
 #  Parent : [composite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/composite.markdown)

 `read-only`

> Getters / setters.
> ``` lang=cpp, name=Lightning
> var Parent : Composite


---  
 #  SelectTool : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> Easy access to the Select Tool. It's commonly used in other Tools (such as ray casting).
> ``` lang=cpp, name=Lightning
> var SelectTool : Cog


---  
 #  Methods


---  
 

 
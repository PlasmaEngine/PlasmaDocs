 `Component` `UiWidget`



(NOTE) Layouts are in charge of calling UpdateTransform on all children, regardless of whether or not they ignore layouts.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Debug](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilayout.markdown#debug-void)|[ PaddingBottom](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilayout.markdown#paddingbottom-plasma-engin)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)|[uidocklayout](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uidocklayout.markdown)|
| |[ PaddingLeft](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilayout.markdown#paddingleft-plasma-engine)| |[uifilllayout](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uifilllayout.markdown)|
| |[ PaddingRight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilayout.markdown#paddingright-plasma-engine)| |[uistacklayout](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uistacklayout.markdown)|
| |[ PaddingTop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilayout.markdown#paddingtop-plasma-engine-d)| | |


 #  Properties


---  
 #  PaddingBottom : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var PaddingBottom : Real


---  
 #  PaddingLeft : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Padding getter / setters for binding until we have Thickness binding.
> ``` lang=cpp, name=Lightning
> var PaddingLeft : Real


---  
 #  PaddingRight : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var PaddingRight : Real


---  
 #  PaddingTop : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> ``` lang=cpp, name=Lightning
> var PaddingTop : Real


---  
 #  Methods


---  
 #  Debug : Void

> Calling this will set a breakpoint before the layout is done.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Debug()
> ``` 


---  
 

 
 `Editor`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#addtext-void)|[ BackgroundColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#backgroundcolor-plasma-eng)| | |
|[ ClearText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#cleartext-void)|[ BorderColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#bordercolor-plasma-engine)| | |
|[ SetColorScheme](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#setcolorscheme-void)|[ Padding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#padding-plasma-engine-docu)| | |
|[ SetPlacement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#setplacement-void)| | | |
|[ SetPriority](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#setpriority-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md#uilegacytooltip-void)| | | |


 #  Properties


---  
 #  BackgroundColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var BackgroundColor : Real4


---  
 #  BorderColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var BorderColor : Real4


---  
 #  Padding : [thickness](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thickness.md)

> 
> ``` lang=cpp, name=Lightning
> var Padding : Thickness


---  
 #  Methods


---  
 #  AddText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |p1|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function AddText(p0 : String, p1 : Real4)
> ``` 


---  
 #  ClearText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearText()
> ``` 


---  
 #  SetColorScheme : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ToolTipColorScheme](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#tooltipcolorscheme)| |
> ``` lang=cpp, name=Lightning
> function SetColorScheme(p0 : ToolTipColorScheme)
> ``` 


---  
 #  SetPlacement : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cameraviewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.md)| |
> |p1|[rectangle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rectangle.md)| |
> ``` lang=cpp, name=Lightning
> function SetPlacement(p0 : CameraViewport, p1 : Rectangle)
> ``` 


---  
 #  SetPriority : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[IndicatorSide](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#indicatorside)| |
> |p1|[IndicatorSide](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#indicatorside)| |
> |p2|[IndicatorSide](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#indicatorside)| |
> |p3|[IndicatorSide](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#indicatorside)| |
> ``` lang=cpp, name=Lightning
> function SetPriority(p0 : IndicatorSide, p1 : IndicatorSide, p2 : IndicatorSide, p3 : IndicatorSide)
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UiLegacyToolTip()
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[uilegacytooltip](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uilegacytooltip.md)| |
> ``` lang=cpp, name=Lightning
> function UiLegacyToolTip(p0 : UiLegacyToolTip)
> ``` 


---  
 

 
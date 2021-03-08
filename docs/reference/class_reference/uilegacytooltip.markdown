 `Editor`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddText](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#addtext-void)|[ BackgroundColor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#backgroundcolor-plasma-eng)| | |
|[ ClearText](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#cleartext-void)|[ BorderColor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#bordercolor-plasma-engine)| | |
|[ SetColorScheme](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#setcolorscheme-void)|[ Padding](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#padding-plasma-engine-docu)| | |
|[ SetPlacement](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#setplacement-void)| | | |
|[ SetPriority](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#setpriority-void)| | | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown#uilegacytooltip-void)| | | |


 #  Properties


---  
 #  BackgroundColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var BackgroundColor : Real4


---  
 #  BorderColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var BorderColor : Real4


---  
 #  Padding : [thickness](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/thickness.markdown)

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
> |p0|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |p1|[real4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)| |
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
> |p0|[ToolTipColorScheme](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#tooltipcolorscheme)| |
> ``` lang=cpp, name=Lightning
> function SetColorScheme(p0 : ToolTipColorScheme)
> ``` 


---  
 #  SetPlacement : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cameraviewport](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown)| |
> |p1|[rectangle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rectangle.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetPlacement(p0 : CameraViewport, p1 : Rectangle)
> ``` 


---  
 #  SetPriority : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[IndicatorSide](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#indicatorside)| |
> |p1|[IndicatorSide](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#indicatorside)| |
> |p2|[IndicatorSide](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#indicatorside)| |
> |p3|[IndicatorSide](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#indicatorside)| |
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
> |p0|[uilegacytooltip](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uilegacytooltip.markdown)| |
> ``` lang=cpp, name=Lightning
> function UiLegacyToolTip(p0 : UiLegacyToolTip)
> ``` 


---  
 

 
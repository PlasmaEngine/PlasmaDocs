 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Render](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#render-void)|[ DebugMouseInteraction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#debugmouseinteraction-ze)|[uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#uirootwidget-void)|[ DebugSelected](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#debugselected-plasma-engin)| | |
|[ Update](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#update-void)|[ DepthSeparation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#depthseparation-plasma-eng)| | |
| |[ DoubleClickTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#doubleclicktime-plasma-eng)| | |
| |[ FocusWidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#focuswidget-plasma-engine)| | |
| |[ MouseDownWidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#mousedownwidget-plasma-eng)| | |
| |[ MouseHoldTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#mouseholdtime-plasma-engin)| | |
| |[ MouseHoverTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#mousehovertime-plasma-engi)| | |
| |[ MouseOverWidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uirootwidget.md#mouseoverwidget-plasma-eng)| | |


 #  Properties


---  
 #  DebugMouseInteraction : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not to print out debug information to the console about what the mouse is currently doing.
> ``` lang=cpp, name=Lightning
> var DebugMouseInteraction : Boolean


---  
 #  DebugSelected : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> ``` lang=cpp, name=Lightning
> var DebugSelected : Cog


---  
 #  DepthSeparation : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Used for debugging.
> ``` lang=cpp, name=Lightning
> var DepthSeparation : Real


---  
 #  DoubleClickTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The amount of time between clicks to send the 'DoubleClick' event.
> ``` lang=cpp, name=Lightning
> var DoubleClickTime : Real


---  
 #  FocusWidget : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.md)

> The widget that currently has focus.
> ``` lang=cpp, name=Lightning
> var FocusWidget : UiWidget


---  
 #  MouseDownWidget : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.md)

 `read-only`

> The widget that the mouse was pressed down on.
> ``` lang=cpp, name=Lightning
> var MouseDownWidget : UiWidget


---  
 #  MouseHoldTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Only send the 'MouseHold' event when the mouse has been holding on a single widget for this amount of time.
> ``` lang=cpp, name=Lightning
> var MouseHoldTime : Real


---  
 #  MouseHoverTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Only send the MouseHover event when the mouse has been over a single widget for this amount of time.
> ``` lang=cpp, name=Lightning
> var MouseHoverTime : Real


---  
 #  MouseOverWidget : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.md)

 `read-only`

> The widget that the mouse is currently over.
> ``` lang=cpp, name=Lightning
> var MouseOverWidget : UiWidget


---  
 #  Methods


---  
 #  Render : Void

> Renders the Ui to the given color render target. The depth render target must have stencil.
> |Name|Type|Description|
> |---|---|---|
> |e|[rendertasksevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendertasksevent.md)| |
> |color|[rendertarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendertarget.md)| |
> |depth|[rendertarget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendertarget.md)| |
> |renderPass|[materialblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/materialblock.md)| |
> ``` lang=cpp, name=Lightning
> function Render(e : RenderTasksEvent, color : RenderTarget, depth : RenderTarget, renderPass : MaterialBlock)
> ``` 


---  
 #  UiRootWidget : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UiRootWidget()
> ``` 


---  
 #  Update : Void

> Updates all widgets and layouts that need to be updated. This should be called right before rendering.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Update()
> ``` 


---  
 

 
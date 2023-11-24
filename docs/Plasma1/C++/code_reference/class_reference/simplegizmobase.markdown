 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#simplegizmobase-void)|[ Color](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#color-plasma-engine-docume)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)|[arrowgizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/arrowgizmo.markdown)|
| |[ DrawOnTop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#drawontop-plasma-engine-do)| |[ringgizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ringgizmo.markdown)|
| |[ HoverColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#hovercolor-plasma-engine-d)| |[squaregizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/squaregizmo.markdown)|
| |[ MouseInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#mouseinput-plasma-engine-d)| | |
| |[ PickingPriority](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#pickingpriority-plasma-eng)| | |
| |[ UseParentAsViewScaleOrigin](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#useparentasviewscaleorig)| | |
| |[ ViewScaled](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simplegizmobase.markdown#viewscaled-plasma-engine-d)| | |


 #  Properties


---  
 #  Color : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.markdown)

> Display colors.
> ``` lang=cpp, name=Lightning
> var Color : Real4


---  
 #  DrawOnTop : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to draw on top of all objects regardless of depth.
> ``` lang=cpp, name=Lightning
> var DrawOnTop : Boolean


---  
 #  HoverColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var HoverColor : Real4


---  
 #  MouseInput : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Whether or not this Gizmo should receive mouse input.
> ``` lang=cpp, name=Lightning
> var MouseInput : Boolean


---  
 #  PickingPriority : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Used to manually determine which Gizmo gets selected when the mouse is over multiple Gizmos. Higher priority will get picked first.
> ``` lang=cpp, name=Lightning
> var PickingPriority : Integer


---  
 #  UseParentAsViewScaleOrigin : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If enabled, the gizmo will scale around it's parent.
> ``` lang=cpp, name=Lightning
> var UseParentAsViewScaleOrigin : Boolean


---  
 #  ViewScaled : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If enabled, the size of the gizmo will stay the same regardless of how far away the camera is.
> ``` lang=cpp, name=Lightning
> var ViewScaled : Boolean


---  
 #  Methods


---  
 #  SimpleGizmoBase : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SimpleGizmoBase()
> ``` 


---  
 

 
 `Component` `Editor`



(NOTE) Registers itself with the GizmoSpace. This allows GizmoSpace to keep track of which Gizmo the mouse is over, as well as send other input events directly to Gizmos.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gizmo.markdown#gizmo-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gizmo.markdown#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
| |[ EditingObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gizmo.markdown#editingobject-plasma-engin)| | |
| |[ ForwardEventsToChildren](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gizmo.markdown#forwardeventstochildren)| | |
| |[ MouseOver](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gizmo.markdown#mouseover-plasma-engine-do)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> If set to false, it will not receive input events.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  EditingObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> Needed?
> ``` lang=cpp, name=Lightning
> var EditingObject : Cog


---  
 #  ForwardEventsToChildren : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> You may want to manually forward the input events to specific children.
> ``` lang=cpp, name=Lightning
> var ForwardEventsToChildren : Boolean


---  
 #  MouseOver : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Whether or not the mouse is currently over the gizmo.
> ``` lang=cpp, name=Lightning
> var MouseOver : Boolean


---  
 #  Methods


---  
 #  Gizmo : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Gizmo()
> ``` 


---  
 

 
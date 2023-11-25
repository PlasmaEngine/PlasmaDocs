 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RayCast](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#raycast-plasma-engine-docu)|[ ArchetypeSelect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#archetypeselect-plasma-eng)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#selecttool-void)|[ Raycaster](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#raycaster-plasma-engine-do)| | |
|[ SmartSelect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#smartselect-plasma-engine)|[ RootSelect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#rootselect-plasma-engine-d)| | |
| |[ SmartGroupSelect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selecttool.md#smartgroupselect-plasma-en)| | |


 #  Properties


---  
 #  ArchetypeSelect : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Selects the root archetype of the tree, subsequent clicks will select the nearest archetype followed by any direct children following that.
> ``` lang=cpp, name=Lightning
> var ArchetypeSelect : Boolean


---  
 #  Raycaster : [raycaster](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/raycaster.md)

> 
> ``` lang=cpp, name=Lightning
> var Raycaster : Raycaster


---  
 #  RootSelect : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Selects the root of a hierarchy first, subsequent clicks will select children objects.
> ``` lang=cpp, name=Lightning
> var RootSelect : Boolean


---  
 #  SmartGroupSelect : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If a parent of a hierarchy is already selected drag select will only select all the children of the currently selected parent.
> ``` lang=cpp, name=Lightning
> var SmartGroupSelect : Boolean


---  
 #  Methods


---  
 #  RayCast : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |viewport|[viewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewport.md)| |
> |mousePosition|[real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)| |
> ``` lang=cpp, name=Lightning
> function RayCast(viewport : Viewport, mousePosition : Real2) : Cog
> ``` 


---  
 #  SelectTool : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SelectTool()
> ``` 


---  
 #  SmartSelect : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |selection|[metaselection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/metaselection.md)| |
> |toSelect|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |rootSelect|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> |archetypeSelect|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function SmartSelect(selection : MetaSelection, toSelect : Cog, rootSelect : Boolean, archetypeSelect : Boolean) : Cog
> ``` 


---  
 

 
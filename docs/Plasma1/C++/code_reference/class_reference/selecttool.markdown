 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RayCast](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#raycast-plasma-engine-docu)|[ ArchetypeSelect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#archetypeselect-plasma-eng)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#selecttool-void)|[ Raycaster](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#raycaster-plasma-engine-do)| | |
|[ SmartSelect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#smartselect-plasma-engine)|[ RootSelect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#rootselect-plasma-engine-d)| | |
| |[ SmartGroupSelect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selecttool.markdown#smartgroupselect-plasma-en)| | |


 #  Properties


---  
 #  ArchetypeSelect : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Selects the root archetype of the tree, subsequent clicks will select the nearest archetype followed by any direct children following that.
> ``` lang=cpp, name=Lightning
> var ArchetypeSelect : Boolean


---  
 #  Raycaster : [raycaster](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/raycaster.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Raycaster : Raycaster


---  
 #  RootSelect : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Selects the root of a hierarchy first, subsequent clicks will select children objects.
> ``` lang=cpp, name=Lightning
> var RootSelect : Boolean


---  
 #  SmartGroupSelect : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> If a parent of a hierarchy is already selected drag select will only select all the children of the currently selected parent.
> ``` lang=cpp, name=Lightning
> var SmartGroupSelect : Boolean


---  
 #  Methods


---  
 #  RayCast : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |viewport|[viewport](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/viewport.markdown)| |
> |mousePosition|[real2](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real2.markdown)| |
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
 #  SmartSelect : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |selection|[metaselection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/metaselection.markdown)| |
> |toSelect|[cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)| |
> |rootSelect|[boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)| |
> |archetypeSelect|[boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function SmartSelect(selection : MetaSelection, toSelect : Cog, rootSelect : Boolean, archetypeSelect : Boolean) : Cog
> ``` 


---  
 

 
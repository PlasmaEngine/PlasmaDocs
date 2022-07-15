 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetChildren](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#getchildren-plasma-engine)|[ ChildCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#childcount-plasma-engine-d)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)|[uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)|
|[ IsAncestorOf](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#isancestorof-plasma-engine)|[ LastDeepestChild](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#lastdeepestchild-plasma-en)| | |
|[ IsDescendantOf](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#isdescendantof-plasma-engi)|[ LastDirectChild](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#lastdirectchild-plasma-eng)| | |
| |[ NextInHierarchyOrder](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#nextinhierarchyorder-zer)| | |
| |[ NextSibling](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#nextsibling-plasma-engine)| | |
| |[ Parent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#parent-plasma-engine-docum)| | |
| |[ PreviousInHierarchyOrder](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#previousinhierarchyorder)| | |
| |[ PreviousSibling](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#previoussibling-plasma-eng)| | |
| |[ Root](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#root-plasma-engine-documen)| | |


 #  Properties


---  
 #  ChildCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ChildCount : Integer


---  
 #  LastDeepestChild : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var LastDeepestChild : UiWidget


---  
 #  LastDirectChild : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var LastDirectChild : UiWidget


---  
 #  NextInHierarchyOrder : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var NextInHierarchyOrder : UiWidget


---  
 #  NextSibling : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var NextSibling : UiWidget


---  
 #  Parent : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Parent : UiWidget


---  
 #  PreviousInHierarchyOrder : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var PreviousInHierarchyOrder : UiWidget


---  
 #  PreviousSibling : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var PreviousSibling : UiWidget


---  
 #  Root : [uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Root : UiWidget


---  
 #  Methods


---  
 #  GetChildren : [uiwidgetrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidgetrange.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetChildren() : UiWidgetRange
> ``` 


---  
 #  IsAncestorOf : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsAncestorOf( : UiWidget) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsDescendantOf( : UiWidget) : Boolean
> ``` 


---  
 

 
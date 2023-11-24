 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetChildren](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#getchildren-plasma-engine)|[ ChildCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#childcount-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)|[uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)|
|[ IsAncestorOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#isancestorof-plasma-engine)|[ LastDeepestChild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#lastdeepestchild-plasma-en)| | |
|[ IsDescendantOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#isdescendantof-plasma-engi)|[ LastDirectChild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#lastdirectchild-plasma-eng)| | |
| |[ NextInHierarchyOrder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#nextinhierarchyorder-zer)| | |
| |[ NextSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#nextsibling-plasma-engine)| | |
| |[ Parent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#parent-plasma-engine-docum)| | |
| |[ PreviousInHierarchyOrder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#previousinhierarchyorder)| | |
| |[ PreviousSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#previoussibling-plasma-eng)| | |
| |[ Root](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetcomponenthierarchy.markdown#root-plasma-engine-documen)| | |


 #  Properties


---  
 #  ChildCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ChildCount : Integer


---  
 #  LastDeepestChild : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var LastDeepestChild : UiWidget


---  
 #  LastDirectChild : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var LastDirectChild : UiWidget


---  
 #  NextInHierarchyOrder : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var NextInHierarchyOrder : UiWidget


---  
 #  NextSibling : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var NextSibling : UiWidget


---  
 #  Parent : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Parent : UiWidget


---  
 #  PreviousInHierarchyOrder : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var PreviousInHierarchyOrder : UiWidget


---  
 #  PreviousSibling : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var PreviousSibling : UiWidget


---  
 #  Root : [uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Root : UiWidget


---  
 #  Methods


---  
 #  GetChildren : [uiwidgetrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidgetrange.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetChildren() : UiWidgetRange
> ``` 


---  
 #  IsAncestorOf : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsAncestorOf( : UiWidget) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uiwidget.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsDescendantOf( : UiWidget) : Boolean
> ``` 


---  
 

 
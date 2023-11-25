 `Resource` `Graphics`



(NOTE) How Materials are categorized, determines which graphicals are drawn in a render pass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsSubRenderGroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#issubrendergroup-plasma-en)|[ ChildRenderGroups](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#childrendergroups-plasma-e)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
|[ IsSubRenderGroupOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#issubrendergroupof-plasma)|[ GraphicalSortMethod](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#graphicalsortmethod-plasma)| | |
| |[ Materials](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#materials-plasma-engine-do)| | |
| |[ ParentRenderGroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#parentrendergroup-plasma-e)| | |
| |[ ReferencedByList](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md#referencedbylist-plasma-en)| | |


 #  Properties


---  
 #  ChildRenderGroups : [childrendergrouplist](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/childrendergrouplist.md)

 `read-only`

> For assigning child RenderGroups, making this a parent group of everything in the list.
> ``` lang=cpp, name=Lightning
> var ChildRenderGroups : ChildRenderGroupList


---  
 #  GraphicalSortMethod : [GraphicalSortMethod](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#graphicalsortmethod)

> Determines the order that graphicals will be drawn when processed as this RenderGroup.
> ``` lang=cpp, name=Lightning
> var GraphicalSortMethod : GraphicalSortMethod


---  
 #  Materials : [materiallist](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/materiallist.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Materials : MaterialList


---  
 #  ParentRenderGroup : [rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)

> RenderGroup that this is a sub group of. Also a sub group of all of its parents.
> ``` lang=cpp, name=Lightning
> var ParentRenderGroup : RenderGroup


---  
 #  ReferencedByList : [materiallist](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/materiallist.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ReferencedByList : MaterialList


---  
 #  Methods


---  
 #  IsSubRenderGroup : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not the given RenderGroup is a sub group of this.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Lightning
> function IsSubRenderGroup(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 #  IsSubRenderGroupOf : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not this is a sub group of the given RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Lightning
> function IsSubRenderGroupOf(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 

 
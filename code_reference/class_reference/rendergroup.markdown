 `Resource` `Graphics`



(NOTE) How Materials are categorized, determines which graphicals are drawn in a render pass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsSubRenderGroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#issubrendergroup-plasma-en)|[ ChildRenderGroups](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#childrendergroups-plasma-e)|[dataresource](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dataresource.markdown)| |
|[ IsSubRenderGroupOf](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#issubrendergroupof-plasma)|[ GraphicalSortMethod](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#graphicalsortmethod-plasma)| | |
| |[ Materials](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#materials-plasma-engine-do)| | |
| |[ ParentRenderGroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#parentrendergroup-plasma-e)| | |
| |[ ReferencedByList](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown#referencedbylist-plasma-en)| | |


 #  Properties


---  
 #  ChildRenderGroups : [childrendergrouplist](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/childrendergrouplist.markdown)

 `read-only`

> For assigning child RenderGroups, making this a parent group of everything in the list.
> ``` lang=cpp, name=Lightning
> var ChildRenderGroups : ChildRenderGroupList


---  
 #  GraphicalSortMethod : [GraphicalSortMethod](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#graphicalsortmethod)

> Determines the order that graphicals will be drawn when processed as this RenderGroup.
> ``` lang=cpp, name=Lightning
> var GraphicalSortMethod : GraphicalSortMethod


---  
 #  Materials : [materiallist](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/materiallist.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Materials : MaterialList


---  
 #  ParentRenderGroup : [rendergroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown)

> RenderGroup that this is a sub group of. Also a sub group of all of its parents.
> ``` lang=cpp, name=Lightning
> var ParentRenderGroup : RenderGroup


---  
 #  ReferencedByList : [materiallist](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/materiallist.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ReferencedByList : MaterialList


---  
 #  Methods


---  
 #  IsSubRenderGroup : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns whether or not the given RenderGroup is a sub group of this.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsSubRenderGroup(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 #  IsSubRenderGroupOf : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns whether or not this is a sub group of the given RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/rendergroup.markdown)| |
> ``` lang=cpp, name=Lightning
> function IsSubRenderGroupOf(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 

 
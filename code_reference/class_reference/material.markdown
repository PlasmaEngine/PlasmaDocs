 `Resource` `Graphics`



(NOTE) A composition of shader fragments that defines a shader program that is used when rendering Graphicals.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RuntimeClone](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/material.markdown#runtimeclone-plasma-engine)|[ CompositionLabel](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/material.markdown#compositionlabel-plasma-en)|[dataresource](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dataresource.markdown)| |
| |[ ReferencedByList](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/material.markdown#referencedbylist-plasma-en)| | |
| |[ RenderGroups](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/material.markdown#rendergroups-plasma-engine)| | |


 #  Properties


---  
 #  CompositionLabel : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CompositionLabel : Integer


---  
 #  ReferencedByList : [rendergrouplist](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/rendergrouplist.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ReferencedByList : RenderGroupList


---  
 #  RenderGroups : [rendergrouplist](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/rendergrouplist.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var RenderGroups : RenderGroupList


---  
 #  Methods


---  
 #  RuntimeClone : [material](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/material.markdown)

> Creates an anonymous copy that can be independently modified, destroyed when all references are gone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : Material
> ``` 


---  
 

 
 `Resource` `Graphics`



(NOTE) A composition of shader fragments that defines a shader program that is used when rendering Graphicals.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md#runtimeclone-plasma-engine)|[ CompositionLabel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md#compositionlabel-plasma-en)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
| |[ ReferencedByList](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md#referencedbylist-plasma-en)| | |
| |[ RenderGroups](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md#rendergroups-plasma-engine)| | |


 #  Properties


---  
 #  CompositionLabel : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var CompositionLabel : Integer


---  
 #  ReferencedByList : [rendergrouplist](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergrouplist.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var ReferencedByList : RenderGroupList


---  
 #  RenderGroups : [rendergrouplist](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergrouplist.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var RenderGroups : RenderGroupList


---  
 #  Methods


---  
 #  RuntimeClone : [material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/material.md)

> Creates an anonymous copy that can be independently modified, destroyed when all references are gone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : Material
> ``` 


---  
 

 
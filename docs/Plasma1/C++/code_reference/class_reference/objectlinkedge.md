 `Engine`

(NOTE) A directed edge between a cog and an object link.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlinkedge.md#objectlinkedge-void)|[ ObjectLink](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlinkedge.md#objectlink-plasma-engine-d)| | |
| |[ OtherCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlinkedge.md#othercog-plasma-engine-doc)| | |
| |[ SelfCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlinkedge.md#selfcog-plasma-engine-docu)| | |


 #  Properties


---  
 #  ObjectLink : [objectlink](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md)

 `read-only`

> The object link that this edge is connected to.
> ``` lang=cpp, name=Lightning
> var ObjectLink : ObjectLink


---  
 #  OtherCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The other cog that the object link is connected to (the one not part of this edge).
> ``` lang=cpp, name=Lightning
> var OtherCog : Cog


---  
 #  SelfCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> The cog that this edge on the object link is connected to.
> ``` lang=cpp, name=Lightning
> var SelfCog : Cog


---  
 #  Methods


---  
 #  ObjectLinkEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ObjectLinkEdge()
> ``` 


---  
 #  ObjectLinkEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[objectlinkedge](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlinkedge.md)| |
> ``` lang=cpp, name=Lightning
> function ObjectLinkEdge( : ObjectLinkEdge)
> ``` 


---  
 

 
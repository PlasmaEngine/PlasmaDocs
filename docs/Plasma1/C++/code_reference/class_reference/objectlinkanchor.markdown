 `Component` `Engine`



(NOTE) Component used to keep track of what ObjectLinks a cog has. This component is added dynamically whenever a ObjectLink is added to a cog that did not contain an ObjectLink before. This can be used to traverse across linked objects and find the entire "island" of ObjectLinks.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlinkanchor.markdown#objectlinkanchor-void)|[ ObjectLinks](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlinkanchor.markdown#objectlinks-plasma-engine)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |


 #  Properties


---  
 #  ObjectLinks : [objectlinkrange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlinkrange.markdown)

 `read-only`

> The range of object link edges connected to this anchor.
> ``` lang=cpp, name=Lightning
> var ObjectLinks : ObjectLinkRange


---  
 #  Methods


---  
 #  ObjectLinkAnchor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ObjectLinkAnchor()
> ``` 


---  
 

 
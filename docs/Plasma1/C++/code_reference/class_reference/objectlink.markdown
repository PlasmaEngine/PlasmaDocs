 `Component` `Engine`



(NOTE) Forms a link between two positions on two objects. ObjectLinks are used primarily by physics to represent joints, but can also be used by graphics, gameplay, etc... to represent some connection between two objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#objectlink-void)|[ LocalPointA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#localpointa-plasma-engine)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |
| |[ LocalPointB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#localpointb-plasma-engine)| | |
| |[ ObjectA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#objecta-plasma-engine-docu)| | |
| |[ ObjectAPath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#objectapath-plasma-engine)| | |
| |[ ObjectB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#objectb-plasma-engine-docu)| | |
| |[ ObjectBPath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#objectbpath-plasma-engine)| | |
| |[ WorldPointA](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/objectlink.markdown#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The Point on Object A in local space.
> ``` lang=cpp, name=Lightning
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The Point on Object B in local space.
> ``` lang=cpp, name=Lightning
> var LocalPointB : Real3


---  
 #  ObjectA : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> The first object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Lightning
> var ObjectA : Cog


---  
 #  ObjectAPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)

> CogPath to object A.
> ``` lang=cpp, name=Lightning
> var ObjectAPath : CogPath


---  
 #  ObjectB : [cog](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cog.markdown)

> The second object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Lightning
> var ObjectB : Cog


---  
 #  ObjectBPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/cogpath.markdown)

> CogPath to object B.
> ``` lang=cpp, name=Lightning
> var ObjectBPath : CogPath


---  
 #  WorldPointA : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The point on object A in world space.
> ``` lang=cpp, name=Lightning
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real3.markdown)

> The point on object B in world space.
> ``` lang=cpp, name=Lightning
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  ObjectLink : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ObjectLink()
> ``` 


---  
 

 
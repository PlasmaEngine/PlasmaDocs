 `Component` `Engine`



(NOTE) Forms a link between two positions on two objects. ObjectLinks are used primarily by physics to represent joints, but can also be used by graphics, gameplay, etc... to represent some connection between two objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#objectlink-void)|[ LocalPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#localpointa-plasma-engine)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ LocalPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#localpointb-plasma-engine)| | |
| |[ ObjectA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#objecta-plasma-engine-docu)| | |
| |[ ObjectAPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#objectapath-plasma-engine)| | |
| |[ ObjectB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#objectb-plasma-engine-docu)| | |
| |[ ObjectBPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#objectbpath-plasma-engine)| | |
| |[ WorldPointA](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#worldpointa-plasma-engine)| | |
| |[ WorldPointB](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md#worldpointb-plasma-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The Point on Object A in local space.
> ``` lang=cpp, name=Lightning
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The Point on Object B in local space.
> ``` lang=cpp, name=Lightning
> var LocalPointB : Real3


---  
 #  ObjectA : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> The first object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Lightning
> var ObjectA : Cog


---  
 #  ObjectAPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

> CogPath to object A.
> ``` lang=cpp, name=Lightning
> var ObjectAPath : CogPath


---  
 #  ObjectB : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> The second object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Lightning
> var ObjectB : Cog


---  
 #  ObjectBPath : [cogpath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cogpath.md)

> CogPath to object B.
> ``` lang=cpp, name=Lightning
> var ObjectBPath : CogPath


---  
 #  WorldPointA : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The point on object A in world space.
> ``` lang=cpp, name=Lightning
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

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
 

 
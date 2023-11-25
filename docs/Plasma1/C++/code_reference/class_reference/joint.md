 `Component` `Physics`



(NOTE) Joints connect two objects together with one or more constraints. A constraint is a mathematical rule that restricts object movement, typically defined in terms of the position and velocities of the objects involved.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#getcog-plasma-engine-docum)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)|[customjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md)|
|[ GetOtherObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#getotherobject-plasma-engi)|[ AutoSnaps](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#autosnaps-plasma-engine-do)| |[fixedanglejoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/fixedanglejoint.md)|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#joint-void)|[ CollideConnected](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#collideconnected-plasma-en)| |[gearjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md)|
| |[ MaxImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#maximpulse-plasma-engine-d)| |[linearaxisjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearaxisjoint.md)|
| |[ SendsEvents](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md#sendsevents-plasma-engine)| |[manipulatorjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjoint.md)|
| | | |[phygunjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/phygunjoint.md)|
| | | |[positionjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md)|
| | | |[prismaticjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint.md)|
| | | |[prismaticjoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md)|
| | | |[pulleyjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.md)|
| | | |[relativevelocityjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md)|
| | | |[revolutejoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint.md)|
| | | |[revolutejoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint2d.md)|
| | | |[stickjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/stickjoint.md)|
| | | |[universaljoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md)|
| | | |[uprightjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.md)|
| | | |[weldjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/weldjoint.md)|
| | | |[wheeljoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint.md)|
| | | |[wheeljoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint2d.md)|


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this joint is currently active. Used for runtime enabling/disabling of joints.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AutoSnaps : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this joint will automatically delete itself if any of its constraints reach the max impulse value. This will still send an event if it snaps.
> ``` lang=cpp, name=Lightning
> var AutoSnaps : Boolean


---  
 #  CollideConnected : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if the two objects connected by this joint can collide. If any joint between this pair does not collide, then the pair does not collide. All joints have to be set to true in order to have the objects collide.
> ``` lang=cpp, name=Lightning
> var CollideConnected : Boolean


---  
 #  MaxImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The maximum impulse (instantaneous force) that this joint can apply to correct itself.
> ``` lang=cpp, name=Lightning
> var MaxImpulse : Real


---  
 #  SendsEvents : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this joint will send any events. Used for a small efficiency boost and for reducing the number of events.
> ``` lang=cpp, name=Lightning
> var SendsEvents : Boolean


---  
 #  Methods


---  
 #  GetCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Returns the cog associated with an index. Index of 0 is ObjectA, index 1 is ObjectB. Used to write more streamline functions where you index into the objects in a loop.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetCog(index : Integer) : Cog
> ``` 


---  
 #  GetOtherObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> If the passed in object is ObjectA, returns ObjectB. Provides easier logic for traversing across joints.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function GetOtherObject(cog : Cog) : Cog
> ``` 


---  
 #  Joint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Joint()
> ``` 


---  
 

 
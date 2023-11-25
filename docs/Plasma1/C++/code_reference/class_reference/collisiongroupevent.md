 `Event` `Physics`



(NOTE) An event sent out when specified by a CollisionFilter in a CollisionTable. Used to hook up events based upon certain CollisionGroup types colliding.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FirstPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.md#firstpoint-plasma-engine-d)|[basecollisionevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.md)| |
| |[ TypeAName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.md#typeaname-plasma-engine-do)| | |
| |[ TypeBName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.md#typebname-plasma-engine-do)| | |


 #  Properties


---  
 #  FirstPoint : [contactpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactpoint.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var FirstPoint : ContactPoint


---  
 #  TypeAName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object A.
> ``` lang=cpp, name=Lightning
> var TypeAName : String


---  
 #  TypeBName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object B.
> ``` lang=cpp, name=Lightning
> var TypeBName : String


---  
 #  Methods


---  
 

 
 `Event` `Physics`



(NOTE) An event sent out when specified by a CollisionFilter in a CollisionTable. Used to hook up events based upon certain CollisionGroup types colliding.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FirstPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.markdown#firstpoint-plasma-engine-d)|[basecollisionevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecollisionevent.markdown)| |
| |[ TypeAName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.markdown#typeaname-plasma-engine-do)| | |
| |[ TypeBName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroupevent.markdown#typebname-plasma-engine-do)| | |


 #  Properties


---  
 #  FirstPoint : [contactpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactpoint.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var FirstPoint : ContactPoint


---  
 #  TypeAName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Returns the CollisionGroup name of object A.
> ``` lang=cpp, name=Lightning
> var TypeAName : String


---  
 #  TypeBName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Returns the CollisionGroup name of object B.
> ``` lang=cpp, name=Lightning
> var TypeBName : String


---  
 #  Methods


---  
 

 
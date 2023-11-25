 `Physics`

(NOTE) Filter for casting operations in physics. Allows basic filtering such as static or dynamic objects, advanced filters such as collision groups, and custom filters via an event callback.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md#castfilter-void)|[ CallbackEventName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md#callbackeventname-plasma-e)|[basecastfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md)| |
| |[ CallbackObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md#callbackobject-object)| | |
| |[ CollisionGroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md#collisiongroup-plasma-engi)| | |
| |[ IgnoreCog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md#ignorecog-plasma-engine-do)| | |


 #  Properties


---  
 #  CallbackEventName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> The name of the event to invoke on the callback object.
> ``` lang=cpp, name=Lightning
> var CallbackEventName : String


---  
 #  CallbackObject : Object

> An object to invoke a callback on (via the callback name) to see if an object in a cast should be skipped.
> ``` lang=cpp, name=Lightning
> var CallbackObject : Object


---  
 #  CollisionGroup : [collisiongroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collisiongroup.md)

> Should this cast behave like it belongs to a collision group? Uses the current space's CollisionTable for filtering logic.
> ``` lang=cpp, name=Lightning
> var CollisionGroup : CollisionGroup


---  
 #  IgnoreCog : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> A cog to ignore during casts.
> ``` lang=cpp, name=Lightning
> var IgnoreCog : Cog


---  
 #  Methods


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CastFilter()
> ``` 


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Lightning
> function CastFilter( : CastFilter)
> ``` 


---  
 

 
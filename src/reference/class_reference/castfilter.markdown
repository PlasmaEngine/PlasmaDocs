 `Physics`

(NOTE) Filter for casting operations in physics. Allows basic filtering such as static or dynamic objects, advanced filters such as collision groups, and custom filters via an event callback.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown#castfilter-void)|[ CallbackEventName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown#callbackeventname-plasma-e)|[basecastfilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown)| |
| |[ CallbackObject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown#callbackobject-object)| | |
| |[ CollisionGroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown#collisiongroup-plasma-engi)| | |
| |[ IgnoreCog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown#ignorecog-plasma-engine-do)| | |


 #  Properties


---  
 #  CallbackEventName : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> The name of the event to invoke on the callback object.
> ``` lang=cpp, name=Lightning
> var CallbackEventName : String


---  
 #  CallbackObject : Object

> An object to invoke a callback on (via the callback name) to see if an object in a cast should be skipped.
> ``` lang=cpp, name=Lightning
> var CallbackObject : Object


---  
 #  CollisionGroup : [collisiongroup](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collisiongroup.markdown)

> Should this cast behave like it belongs to a collision group? Uses the current space's CollisionTable for filtering logic.
> ``` lang=cpp, name=Lightning
> var CollisionGroup : CollisionGroup


---  
 #  IgnoreCog : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

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
> ||[castfilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown)| |
> ``` lang=cpp, name=Lightning
> function CastFilter( : CastFilter)
> ``` 


---  
 

 
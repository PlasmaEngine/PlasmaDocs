 `Component` `Physics`



(NOTE) Regions are used to make PhysicsEffects affect a region of space. Any effects attached to a Cog with a Region will apply to all objects in contact with this region.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.md#dispatchevent-void)|[ WakeUpOnEffectChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.md#wakeuponeffectchange-zer)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.md#region-void)| | | |


 #  Properties


---  
 #  WakeUpOnEffectChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if all objects in the region should be woken up when an effect is changed. Used to make sure that changes in effects will be applied to an object event if it is asleep.
> ``` lang=cpp, name=Lightning
> var WakeUpOnEffectChange : Boolean


---  
 #  Methods


---  
 #  DispatchEvent : Void

> Dispatches an event to all objects in this region.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |toSend|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchEvent(eventId : String, toSend : Event)
> ``` 


---  
 #  Region : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Region()
> ``` 


---  
 

 
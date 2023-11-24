 `Component` `Physics`



(NOTE) A common interface for all effects in physics. An effect is something that typically applies a force and can be attached to a collider, rigid body, region, or even a space. This effect is applied every frame according to the rules of the object it is attached to.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Toggle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown#toggle-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)|[basicdirectioneffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicdirectioneffect.markdown)|
| |[ DebugDrawEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown#debugdraweffect-plasma-eng)| |[basicpointeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicpointeffect.markdown)|
| |[ EffectType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown#effecttype-plasma-engine-d)| |[buoyancyeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/buoyancyeffect.markdown)|
| |[ WakeUpOnChange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown#wakeuponchange-plasma-engi)| |[customphysicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customphysicseffect.markdown)|
| | | |[drageffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.markdown)|
| | | |[floweffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.markdown)|
| | | |[thrusteffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/thrusteffect.markdown)|
| | | |[torqueeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/torqueeffect.markdown)|
| | | |[vortexeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/vortexeffect.markdown)|
| | | |[windeffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/windeffect.markdown)|


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Enable/disable this effect.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  DebugDrawEffect : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Should the effect debug draw.
> ``` lang=cpp, name=Lightning
> var DebugDrawEffect : Boolean


---  
 #  EffectType : [PhysicsEffectType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#physicseffecttype)

 `read-only`

> What kind of effect this is (e.g. ForceEffect, GravityEffect, etc...).
> ``` lang=cpp, name=Lightning
> var EffectType : PhysicsEffectType


---  
 #  WakeUpOnChange : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Whether the object associated with this is woken up when any property is changed.
> ``` lang=cpp, name=Lightning
> var WakeUpOnChange : Boolean


---  
 #  Methods


---  
 #  Toggle : Void

> Toggles whether or not this effect is active.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Toggle()
> ``` 


---  
 

 
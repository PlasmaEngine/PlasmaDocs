 `Component` `Physics`



(NOTE) Allows a cog to ignore certain effect types (such as gravity or drag) that are being applied to the entire space (effects on Space or LevelSettings).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetIgnoreState](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#getignorestate-plasma-engi)|[ IgnoreBuoyancy](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorebuoyancy-plasma-engi)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorespaceeffects-void)|[ IgnoreCustom](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorecustom-plasma-engine)| | |
|[ SetIgnoreState](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#setignorestate-void)|[ IgnoreDrag](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignoredrag-plasma-engine-d)| | |
| |[ IgnoreFlow](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignoreflow-plasma-engine-d)| | |
| |[ IgnoreForce](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignoreforce-plasma-engine)| | |
| |[ IgnoreGravity](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignoregravity-plasma-engin)| | |
| |[ IgnorePointForce](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorepointforce-plasma-en)| | |
| |[ IgnorePointGravity](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorepointgravity-plasma)| | |
| |[ IgnoreThrust](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorethrust-plasma-engine)| | |
| |[ IgnoreTorque](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignoretorque-plasma-engine)| | |
| |[ IgnoreVortex](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorevortex-plasma-engine)| | |
| |[ IgnoreWind](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ignorespaceeffects.markdown#ignorewind-plasma-engine-d)| | |


 #  Properties


---  
 #  IgnoreBuoyancy : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore buoyancy effects.
> ``` lang=cpp, name=Lightning
> var IgnoreBuoyancy : Boolean


---  
 #  IgnoreCustom : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore custom effects.
> ``` lang=cpp, name=Lightning
> var IgnoreCustom : Boolean


---  
 #  IgnoreDrag : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore drag effects.
> ``` lang=cpp, name=Lightning
> var IgnoreDrag : Boolean


---  
 #  IgnoreFlow : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore flow effects.
> ``` lang=cpp, name=Lightning
> var IgnoreFlow : Boolean


---  
 #  IgnoreForce : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore force effects.
> ``` lang=cpp, name=Lightning
> var IgnoreForce : Boolean


---  
 #  IgnoreGravity : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore gravity effects.
> ``` lang=cpp, name=Lightning
> var IgnoreGravity : Boolean


---  
 #  IgnorePointForce : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore point force effects.
> ``` lang=cpp, name=Lightning
> var IgnorePointForce : Boolean


---  
 #  IgnorePointGravity : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore point gravity effects.
> ``` lang=cpp, name=Lightning
> var IgnorePointGravity : Boolean


---  
 #  IgnoreThrust : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore thrust effects.
> ``` lang=cpp, name=Lightning
> var IgnoreThrust : Boolean


---  
 #  IgnoreTorque : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore torque effects.
> ``` lang=cpp, name=Lightning
> var IgnoreTorque : Boolean


---  
 #  IgnoreVortex : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore vortex effects.
> ``` lang=cpp, name=Lightning
> var IgnoreVortex : Boolean


---  
 #  IgnoreWind : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to ignore wind effects.
> ``` lang=cpp, name=Lightning
> var IgnoreWind : Boolean


---  
 #  Methods


---  
 #  GetIgnoreState : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should the given effect type be ignored?
> |Name|Type|Description|
> |---|---|---|
> |effectType|[PhysicsEffectType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#physicseffecttype)| |
> ``` lang=cpp, name=Lightning
> function GetIgnoreState(effectType : PhysicsEffectType) : Boolean
> ``` 


---  
 #  IgnoreSpaceEffects : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IgnoreSpaceEffects()
> ``` 


---  
 #  SetIgnoreState : Void

> Set if an effect type should be ignored.
> |Name|Type|Description|
> |---|---|---|
> |effectType|[PhysicsEffectType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#physicseffecttype)| |
> |ignore|[boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetIgnoreState(effectType : PhysicsEffectType, ignore : Boolean)
> ``` 


---  
 

 
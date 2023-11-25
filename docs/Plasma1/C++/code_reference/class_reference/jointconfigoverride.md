 `Component` `Physics`



(NOTE) Overrides a joint's configuration values of slop, linear/angular Baumgarte, and linear/angular error correction. Slop is the amount of error allowed before position correction takes effect. Baumgarte is used to correct error with a penalty impulse. Baumgarte is split into linear and angular portions because of stability. Error correction is only used when the joint is solved with post stabilization.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#jointconfigoverride-void)|[ AngularBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#angularbaumgarte-plasma-en)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ AngularErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#angularerrorcorrection-z)| | |
| |[ LinearBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#linearbaumgarte-plasma-eng)| | |
| |[ LinearErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#linearerrorcorrection-ze)| | |
| |[ PositionCorrectionType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#positioncorrectiontype-z)| | |
| |[ Slop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md#slop-plasma-engine-documen)| | |


 #  Properties


---  
 #  AngularBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The exponential constant for correcting angular error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The exponential constant for correcting linear error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#constraintpositioncorrection)

> The kind of position correction that this joint should use.
> ``` lang=cpp, name=Lightning
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The amount of error allowed before position correction takes effect.
> ``` lang=cpp, name=Lightning
> var Slop : Real


---  
 #  Methods


---  
 #  JointConfigOverride : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function JointConfigOverride()
> ``` 


---  
 

 
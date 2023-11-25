 `Physics`

(NOTE) Information to represent a constraint to be solved. The main information that needs to be set here is the Jacobian and error. A constraint will enforce that the relative velocities along the Jacobian are equal to plasma (ignoring error correction or motors).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeMotor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#computemotor-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#active-plasma-engine-docum)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)| |
|[ ComputeSpring](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#computespring-void)|[ Angular0](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#angular0-plasma-engine-doc)| | |
|[ DetachFromOwner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#detachfromowner-void)|[ Angular1](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#angular1-plasma-engine-doc)| | |
|[ IsOwned](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#isowned-plasma-engine-docu)|[ Baumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#baumgarte-plasma-engine-do)| | |
|[ SetErrorAndBias](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#seterrorandbias-void)|[ Bias](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#bias-plasma-engine-documen)| | |
|[ SetJacobian](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#setjacobian-void)|[ EffectiveMass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#effectivemass-plasma-engin)| | |
| |[ Error](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#error-plasma-engine-docume)| | |
| |[ Gamma](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#gamma-plasma-engine-docume)| | |
| |[ Impulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#impulse-plasma-engine-docu)| | |
| |[ Linear0](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#linear0-plasma-engine-docu)| | |
| |[ Linear1](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#linear1-plasma-engine-docu)| | |
| |[ MaxImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#maximpulse-plasma-engine-d)| | |
| |[ MinImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#minimpulse-plasma-engine-d)| | |
| |[ Owner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#owner-plasma-engine-docume)| | |
| |[ SolvePosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md#solveposition-plasma-engin)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is this constraint currently active?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  Angular0 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Angular portion of objectA's Jacobian.
> ``` lang=cpp, name=Lightning
> var Angular0 : Real3


---  
 #  Angular1 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Angular portion of objectB's Jacobian.
> ``` lang=cpp, name=Lightning
> var Angular1 : Real3


---  
 #  Baumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The baumgarte term used to correct error. This should typically be set in initialization (per constraint) and then left alone. Default value is 5.
> ``` lang=cpp, name=Lightning
> var Baumgarte : Real


---  
 #  Bias : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The bias is used to apply energy into the system. Typically, bias is combined with Error and Baumgarte to fix error. Bias is also used for motors and springs to drive the constraint.
> ``` lang=cpp, name=Lightning
> var Bias : Real


---  
 #  EffectiveMass : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The effective mass of the constraint. This is typically set by calling SetJacobian.
> ``` lang=cpp, name=Lightning
> var EffectiveMass : Real


---  
 #  Error : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The error of the constraint. This should typically be set via the SetError function.
> ``` lang=cpp, name=Lightning
> var Error : Real


---  
 #  Gamma : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Gamma is used to soften constraints. This should typically never be manually set. Instead, it is set when configuring the constraint to act like a spring.
> ``` lang=cpp, name=Lightning
> var Gamma : Real


---  
 #  Impulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The total accumulated impulse of this constraint. If you want to not use warm-starting then clear this value every frame.
> ``` lang=cpp, name=Lightning
> var Impulse : Real


---  
 #  Linear0 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Linear portion of objectA's Jacobian.
> ``` lang=cpp, name=Lightning
> var Linear0 : Real3


---  
 #  Linear1 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Linear portion of objectB's Jacobian.
> ``` lang=cpp, name=Lightning
> var Linear1 : Real3


---  
 #  MaxImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max impulse magnitude allowed for the constraint.
> ``` lang=cpp, name=Lightning
> var MaxImpulse : Real


---  
 #  MinImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The min impulse magnitude allowed for the constraint.
> ``` lang=cpp, name=Lightning
> var MinImpulse : Real


---  
 #  Owner : [customjoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md)

 `read-only`

> What joint currently owns this constraint.
> ``` lang=cpp, name=Lightning
> var Owner : CustomJoint


---  
 #  SolvePosition : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should this constraint solve position directly or use baumgarte correction? Toggling SolvePosition should be done before setting any other values (ideally in initialization). Setting a constraint to be a motor or a spring will turn off position correction as an error bias must be used to solve those scenarios.
> ``` lang=cpp, name=Lightning
> var SolvePosition : Boolean


---  
 #  Methods


---  
 #  ComputeMotor : Void

> Sets this constraint as a motor (i.e. a constraint that drives movement along the Jacobian direction at a certain speed). The motor has a min and max impulse value that can be solved (typically -value, +value). If you set this as a motor, you should do so last. Motors should typically be their own constraint unlike springs.
> |Name|Type|Description|
> |---|---|---|
> |targetSpeed|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |minImpulse|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |maxImpulse|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function ComputeMotor(targetSpeed : Real, minImpulse : Real, maxImpulse : Real)
> ``` 


---  
 #  ComputeSpring : Void

> Given the currently set mass and error, fix the constraint to be soft (i.e. solve the constraint like a spring). The spring fixes the constraint using the given frequency (oscillations per second) and damping ratio (0 is no damping, 1 is critical damping).
> |Name|Type|Description|
> |---|---|---|
> |frequencyHz|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |dampRatio|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function ComputeSpring(frequencyHz : Real, dampRatio : Real)
> ``` 


---  
 #  DetachFromOwner : Void

> Remove this constraint from whatever joint owns it. This is equivalent to "this.Owner.RemoveConstraint(this)".
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DetachFromOwner()
> ``` 


---  
 #  IsOwned : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is this constraint currently owned by a joint? (Equivalent to "this.Owner != null").
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsOwned() : Boolean
> ``` 


---  
 #  SetErrorAndBias : Void

> Set the position error of the constraint. This also sets the bias of the constraint (used to actually correct the error). If you want to set this constraint as a motor you should not call this function (or call it first). If you want to set this as a spring then make sure you call this first.
> |Name|Type|Description|
> |---|---|---|
> |error|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetErrorAndBias(error : Real)
> ``` 


---  
 #  SetJacobian : Void

> Set the Jacobian of this constraint (and the effective mass).
> |Name|Type|Description|
> |---|---|---|
> |linear0|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |angular0|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |linear1|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |angular1|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function SetJacobian(linear0 : Real3, angular0 : Real3, linear1 : Real3, angular1 : Real3)
> ``` 


---  
 

 
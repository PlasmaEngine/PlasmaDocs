 `Resource` `Physics`



(NOTE) Defines various configuration values used by physics to solve constraints. This resource defines a tiered set of properties that can be overridden global or per constraint type.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md#physicssolverconfig-void)|[ PositionCorrectionType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md#positioncorrectiontype-z)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
| |[ PositionIterationCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md#positioniterationcount-z)| | |
| |[ SolverIterationCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md#solveriterationcount-zer)| | |
| |[ VelocityRestitutionThreshold](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicssolverconfig.md#velocityrestitutionthres)| | |


 #  Properties


---  
 #  PositionCorrectionType : [PhysicsSolverPositionCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#physicssolverpositioncorrection)

> What method should be used to fix errors in joints. Baumgarte fixes errors by adding extra velocity but results in a more spongy behavior. Post Stabilization fixes errors by directly modifying position but can behave worse in unsolvable configurations.
> ``` lang=cpp, name=Lightning
> var PositionCorrectionType : PhysicsSolverPositionCorrection


---  
 #  PositionIterationCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of iterations used for position correction (if position correction is used).
> ``` lang=cpp, name=Lightning
> var PositionIterationCount : Integer


---  
 #  SolverIterationCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of iterations used in the constraint solver. Affects how stiff joints will be.
> ``` lang=cpp, name=Lightning
> var SolverIterationCount : Integer


---  
 #  VelocityRestitutionThreshold : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> To prevent numerical issues, restitution is only applied if the relative velocity between the two objects is above this value.
> ``` lang=cpp, name=Lightning
> var VelocityRestitutionThreshold : Real


---  
 #  Methods


---  
 #  PhysicsSolverConfig : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PhysicsSolverConfig()
> ``` 


---  
 

 
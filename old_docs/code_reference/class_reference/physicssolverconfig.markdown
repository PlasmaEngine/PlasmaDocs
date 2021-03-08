 `Resource` `Physics`



(NOTE) Defines various configuration values used by physics to solve constraints. This resource defines a tiered set of properties that can be overridden global or per constraint type.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicssolverconfig.markdown#physicssolverconfig-void)|[ PositionCorrectionType](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicssolverconfig.markdown#positioncorrectiontype-z)|[dataresource](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/dataresource.markdown)| |
| |[ PositionIterationCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicssolverconfig.markdown#positioniterationcount-z)| | |
| |[ SolverIterationCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicssolverconfig.markdown#solveriterationcount-zer)| | |
| |[ VelocityRestitutionThreshold](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicssolverconfig.markdown#velocityrestitutionthres)| | |


 #  Properties


---  
 #  PositionCorrectionType : [PhysicsSolverPositionCorrection](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#physicssolverpositioncorrection)

> What method should be used to fix errors in joints. Baumgarte fixes errors by adding extra velocity but results in a more spongy behavior. Post Stabilization fixes errors by directly modifying position but can behave worse in unsolvable configurations.
> ``` lang=cpp, name=Lightning
> var PositionCorrectionType : PhysicsSolverPositionCorrection


---  
 #  PositionIterationCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> The number of iterations used for position correction (if position correction is used).
> ``` lang=cpp, name=Lightning
> var PositionIterationCount : Integer


---  
 #  SolverIterationCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> The number of iterations used in the constraint solver. Affects how stiff joints will be.
> ``` lang=cpp, name=Lightning
> var SolverIterationCount : Integer


---  
 #  VelocityRestitutionThreshold : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
 

 
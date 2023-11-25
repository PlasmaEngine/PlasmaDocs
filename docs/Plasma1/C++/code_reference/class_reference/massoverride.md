 `Component` `Physics`



(NOTE) Takes a snap shot of the current mass and inertia and overrides the object's mass so it can be resized while keeping it's old mass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#massoverride-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ RecomputeMass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#recomputemass-void)|[ AutoComputeCenterOfMass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#autocomputecenterofmass)| | |
| |[ AutoComputeInertia](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#autocomputeinertia-plasma)| | |
| |[ InverseMass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#inversemass-plasma-engine)| | |
| |[ LocalCenterOfMass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#localcenterofmass-plasma-e)| | |
| |[ LocalInverseInertiaTensor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#localinverseinertiatenso)| | |
| |[ Mass](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/massoverride.md#mass-plasma-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines whether the RigidBody on this Cog will use the cached or actual mass and inertia.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AutoComputeCenterOfMass : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the center of mass be auto computed or overwritten (via script).
> ``` lang=cpp, name=Lightning
> var AutoComputeCenterOfMass : Boolean


---  
 #  AutoComputeInertia : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the inertia tensor be auto computed or overwritten (via script).
> ``` lang=cpp, name=Lightning
> var AutoComputeInertia : Boolean


---  
 #  InverseMass : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The cached inverse mass of this object.
> ``` lang=cpp, name=Lightning
> var InverseMass : Real


---  
 #  LocalCenterOfMass : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The center of mass in local space to override with. When set, the center of mass will be locked to this value until AutoComputeCenterOfMass is set to true.
> ``` lang=cpp, name=Lightning
> var LocalCenterOfMass : Real3


---  
 #  LocalInverseInertiaTensor : [real3x3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3x3.md)

> The inverse inertia tensor this object is saved with.
> ``` lang=cpp, name=Lightning
> var LocalInverseInertiaTensor : Real3x3


---  
 #  Mass : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Overrides the mass of this body. Inertia is updated as a ratio of the new mass to the old mass.
> ``` lang=cpp, name=Lightning
> var Mass : Real


---  
 #  Methods


---  
 #  MassOverride : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MassOverride()
> ``` 


---  
 #  RecomputeMass : Void

> Takes a new snapshot of the current mass and inertia.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RecomputeMass()
> ``` 


---  
 

 
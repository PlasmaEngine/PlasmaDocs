 `Resource` `Physics`



(NOTE) Describes material properties of a collider mainly used during collision resolution.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#createruntime-plasma-engin)|[ Density](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#density-plasma-engine-docu)|[dataresource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dataresource.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#physicsmaterial-void)|[ Friction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#friction-plasma-engine-doc)| | |
|[ RuntimeClone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#runtimeclone-plasma-engine)|[ FrictionImportance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#frictionimportance-plasma)| | |
|[ UpdateAndNotifyIfModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#updateandnotifyifmodifie)|[ HighPriority](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#highpriority-plasma-engine)| | |
| |[ Restitution](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#restitution-plasma-engine)| | |
| |[ RestitutionImportance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md#restitutionimportance-ze)| | |


 #  Properties


---  
 #  Density : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Density is used to determine the mass of an object. Mass is computed as density * volume. Density can be set to exactly 0 to produce a massless object, however this should only be done with children objects to add collision without affecting mass.
> ``` lang=cpp, name=Lightning
> var Density : Real


---  
 #  Friction : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How slippery or rough the object is. When friction is 0 the object will be slippery. As friction increases, sliding objects will stop quicker. The friction of two object's are combined with the formula sqrt(a * b).
> ``` lang=cpp, name=Lightning
> var Friction : Real


---  
 #  FrictionImportance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Determines which object's friction should be used. If object A's friction importance value is larger than object B's then object A's friction will be used. If both importance values are the same then the default combination logic will be used (see the description of Friction for details).
> ``` lang=cpp, name=Lightning
> var FrictionImportance : Real


---  
 #  HighPriority : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Deprecated. Use RestitutionImportance instead.
> ``` lang=cpp, name=Lightning
> var HighPriority : Boolean


---  
 #  Restitution : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> How much an object will bounce during a collision. Values should be in the range [0,1] where 0 is an inelastic collision and 1 is a fully elastic collision. Restitution is computed as the max of the two objects. Note: due to solving constraints with baumgarte, energy will not be perfectly conserved with a restitution 1.
> ``` lang=cpp, name=Lightning
> var Restitution : Real


---  
 #  RestitutionImportance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Determines which object's restitution should be used. If object A's restitution importance value is larger than object B's then object A's restitution will be used. If both importance values are the same then the default combination logic will be used (see the description of Restitution for details).
> ``` lang=cpp, name=Lightning
> var RestitutionImportance : Real


---  
 #  Methods


---  
 #  CreateRuntime : [physicsmaterial](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md)

 `static`

> Creates a PhysicsMaterial for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateRuntime() : PhysicsMaterial
> ``` 


---  
 #  PhysicsMaterial : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PhysicsMaterial()
> ``` 


---  
 #  RuntimeClone : [physicsmaterial](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsmaterial.md)

> Creates a clone of this material for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RuntimeClone() : PhysicsMaterial
> ``` 


---  
 #  UpdateAndNotifyIfModified : Void

> After modifying this resource, notify anyone using it to update now instead of at the next physics update.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UpdateAndNotifyIfModified()
> ``` 


---  
 

 
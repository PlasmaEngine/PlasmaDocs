 `Physics`

(NOTE) Used to filter objects during cast operations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ IgnoreChildren](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md#ignorechildren-plasma-engi)| |[castfilter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/castfilter.md)|
| |[ IgnoreDynamic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md#ignoredynamic-plasma-engin)| | |
| |[ IgnoreGhost](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md#ignoreghost-plasma-engine)| | |
| |[ IgnoreKinematic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md#ignorekinematic-plasma-eng)| | |
| |[ IgnoreStatic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basecastfilter.md#ignorestatic-plasma-engine)| | |


 #  Properties


---  
 #  IgnoreChildren : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> This flag is currently only used for SweepCollider tests on PhysicsSpace. This is used to ignore all objects that are a child of the Collider that is being swept.
> ``` lang=cpp, name=Lightning
> var IgnoreChildren : Boolean


---  
 #  IgnoreDynamic : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should Colliders with RigidBodies marked Dynamic be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreDynamic : Boolean


---  
 #  IgnoreGhost : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should Colliders marked Ghost be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreGhost : Boolean


---  
 #  IgnoreKinematic : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should Colliders with RigidBodies marked Kinematic be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreKinematic : Boolean


---  
 #  IgnoreStatic : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should Colliders with RigidBodies marked Static be ignored during casts? Note: Collider's with no RigidBody are treated as static.
> ``` lang=cpp, name=Lightning
> var IgnoreStatic : Boolean


---  
 #  Methods


---  
 

 
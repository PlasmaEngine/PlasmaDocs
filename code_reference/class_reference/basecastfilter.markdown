 `Physics`

(NOTE) Used to filter objects during cast operations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ IgnoreChildren](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown#ignorechildren-plasma-engi)| |[castfilter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/castfilter.markdown)|
| |[ IgnoreDynamic](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown#ignoredynamic-plasma-engin)| | |
| |[ IgnoreGhost](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown#ignoreghost-plasma-engine)| | |
| |[ IgnoreKinematic](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown#ignorekinematic-plasma-eng)| | |
| |[ IgnoreStatic](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/basecastfilter.markdown#ignorestatic-plasma-engine)| | |


 #  Properties


---  
 #  IgnoreChildren : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> This flag is currently only used for SweepCollider tests on PhysicsSpace. This is used to ignore all objects that are a child of the Collider that is being swept.
> ``` lang=cpp, name=Lightning
> var IgnoreChildren : Boolean


---  
 #  IgnoreDynamic : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should Colliders with RigidBodies marked Dynamic be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreDynamic : Boolean


---  
 #  IgnoreGhost : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should Colliders marked Ghost be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreGhost : Boolean


---  
 #  IgnoreKinematic : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should Colliders with RigidBodies marked Kinematic be ignored during casts?
> ``` lang=cpp, name=Lightning
> var IgnoreKinematic : Boolean


---  
 #  IgnoreStatic : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Should Colliders with RigidBodies marked Static be ignored during casts? Note: Collider's with no RigidBody are treated as static.
> ``` lang=cpp, name=Lightning
> var IgnoreStatic : Boolean


---  
 #  Methods


---  
 

 
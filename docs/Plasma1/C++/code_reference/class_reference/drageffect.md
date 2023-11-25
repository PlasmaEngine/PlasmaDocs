 `Component` `Physics`



(NOTE) Applies drag or damping forces to slow down an object's linear and angular velocity. Drag is computed as a simple linear approximation of the drag force. Damping is a linear approximation of a drag acceleration. This means that damping affects all objects the same (mass independent).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.md#drageffect-void)|[ AngularDamping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.md#angulardamping-plasma-engi)|[physicseffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)| |
| |[ AngularDrag](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.md#angulardrag-plasma-engine)| | |
| |[ LinearDamping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.md#lineardamping-plasma-engin)| | |
| |[ LinearDrag](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/drageffect.md#lineardrag-plasma-engine-d)| | |


 #  Properties


---  
 #  AngularDamping : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Angular damping coefficient for applying an angular drag acceleration (accel = -kw). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Lightning
> var AngularDamping : Real


---  
 #  AngularDrag : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The angular drag coefficient for applying an angular drag force (T = -kw).
> ``` lang=cpp, name=Lightning
> var AngularDrag : Real


---  
 #  LinearDamping : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Linear damping coefficient for applying a linear drag acceleration (accel = -bv). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Lightning
> var LinearDamping : Real


---  
 #  LinearDrag : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The linear drag coefficient for applying a linear drag force (F = -bv).
> ``` lang=cpp, name=Lightning
> var LinearDrag : Real


---  
 #  Methods


---  
 #  DragEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DragEffect()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) Applies drag or damping forces to slow down an object's linear and angular velocity. Drag is computed as a simple linear approximation of the drag force. Damping is a linear approximation of a drag acceleration. This means that damping affects all objects the same (mass independent).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/drageffect.markdown#drageffect-void)|[ AngularDamping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/drageffect.markdown#angulardamping-plasma-engi)|[physicseffect](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/physicseffect.markdown)| |
| |[ AngularDrag](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/drageffect.markdown#angulardrag-plasma-engine)| | |
| |[ LinearDamping](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/drageffect.markdown#lineardamping-plasma-engin)| | |
| |[ LinearDrag](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/drageffect.markdown#lineardrag-plasma-engine-d)| | |


 #  Properties


---  
 #  AngularDamping : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Angular damping coefficient for applying an angular drag acceleration (accel = -kw). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Lightning
> var AngularDamping : Real


---  
 #  AngularDrag : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The angular drag coefficient for applying an angular drag force (T = -kw).
> ``` lang=cpp, name=Lightning
> var AngularDrag : Real


---  
 #  LinearDamping : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Linear damping coefficient for applying a linear drag acceleration (accel = -bv). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Lightning
> var LinearDamping : Real


---  
 #  LinearDrag : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
 

 
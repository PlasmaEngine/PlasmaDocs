 `Component` `Physics`



(NOTE) A customizable joint that can be configured in script. The user can create constraints belonging to this joint and set the required values to solve them. Some basic constraint understanding is required. To compute constraints you should listen to Events.ComputeCustomJointInfo.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddConstraint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#addconstraint-void)|[ ConstraintCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#constraintcount-plasma-eng)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/joint.markdown)| |
|[ ClearConstraints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#clearconstraints-void)| | | |
|[ CreateConstraint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#createconstraint-plasma-en)| | | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#customjoint-void)| | | |
|[ GetConstraint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#getconstraint-plasma-engin)| | | |
|[ RemoveConstraint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customjoint.markdown#removeconstraint-void)| | | |


 #  Properties


---  
 #  ConstraintCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Returns how many constraints this joint owns.
> ``` lang=cpp, name=Lightning
> var ConstraintCount : Integer


---  
 #  Methods


---  
 #  AddConstraint : Void

> Add a constraint to this joint. This will assert if a joint already owns this constraint.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customconstraintinfo.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 #  ClearConstraints : Void

> Clear all constraints from this joint (so none will solve).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearConstraints()
> ``` 


---  
 #  CreateConstraint : [customconstraintinfo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customconstraintinfo.markdown)

> Create a constraint that is attached to this joint.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateConstraint() : CustomConstraintInfo
> ``` 


---  
 #  CustomJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CustomJoint()
> ``` 


---  
 #  GetConstraint : [customconstraintinfo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customconstraintinfo.markdown)

> Returns the constraint at the given index. Will assert if the index is outside the constraint count range.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetConstraint(index : Integer) : CustomConstraintInfo
> ``` 


---  
 #  RemoveConstraint : Void

> If the given constraint belongs to this joint then remove it from the constraints to solve.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/customconstraintinfo.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 

 
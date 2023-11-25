 `Component` `Physics`



(NOTE) A customizable joint that can be configured in script. The user can create constraints belonging to this joint and set the required values to solve them. Some basic constraint understanding is required. To compute constraints you should listen to Events.ComputeCustomJointInfo.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddConstraint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#addconstraint-void)|[ ConstraintCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#constraintcount-plasma-eng)|[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
|[ ClearConstraints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#clearconstraints-void)| | | |
|[ CreateConstraint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#createconstraint-plasma-en)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#customjoint-void)| | | |
|[ GetConstraint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#getconstraint-plasma-engin)| | | |
|[ RemoveConstraint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md#removeconstraint-void)| | | |


 #  Properties


---  
 #  ConstraintCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

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
> |constraint|[customconstraintinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md)| |
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
 #  CreateConstraint : [customconstraintinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md)

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
 #  GetConstraint : [customconstraintinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md)

> Returns the constraint at the given index. Will assert if the index is outside the constraint count range.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetConstraint(index : Integer) : CustomConstraintInfo
> ``` 


---  
 #  RemoveConstraint : Void

> If the given constraint belongs to this joint then remove it from the constraints to solve.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 

 
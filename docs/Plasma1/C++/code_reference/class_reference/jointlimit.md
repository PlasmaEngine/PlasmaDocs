 `Component` `Physics`



(NOTE) Defines limit properties for a joint. Used to add a min/max bounds to a joint. When the joint is in between the min/max bounds, the "limited" portion will be ignored (The stick will not solve when it is in between the bounds, making it a rope). See each joint for a description of how it reacts to a limit.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md#jointlimit-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ AtomIds](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md#atomids-plasma-engine-docu)| | |
| |[ LowerLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md#lowerlimit-plasma-engine-d)| | |
| |[ UpperLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md#upperlimit-plasma-engine-d)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Determines if this limit is currently active.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AtomIds : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Lightning
> var AtomIds : Integer


---  
 #  LowerLimit : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The lower bound for this limit.
> ``` lang=cpp, name=Lightning
> var LowerLimit : Real


---  
 #  UpperLimit : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The upper bound for this limit.
> ``` lang=cpp, name=Lightning
> var UpperLimit : Real


---  
 #  Methods


---  
 #  JointLimit : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function JointLimit()
> ``` 


---  
 

 
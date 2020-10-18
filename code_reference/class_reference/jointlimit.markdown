 `Component` `Physics`



(NOTE) Defines limit properties for a joint. Used to add a min/max bounds to a joint. When the joint is in between the min/max bounds, the "limited" portion will be ignored (The stick will not solve when it is in between the bounds, making it a rope). See each joint for a description of how it reacts to a limit.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointlimit.markdown#jointlimit-void)|[ Active](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointlimit.markdown#active-plasma-engine-docum)|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
| |[ AtomIds](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointlimit.markdown#atomids-plasma-engine-docu)| | |
| |[ LowerLimit](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointlimit.markdown#lowerlimit-plasma-engine-d)| | |
| |[ UpperLimit](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/jointlimit.markdown#upperlimit-plasma-engine-d)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Determines if this limit is currently active.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AtomIds : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Lightning
> var AtomIds : Integer


---  
 #  LowerLimit : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The lower bound for this limit.
> ``` lang=cpp, name=Lightning
> var LowerLimit : Real


---  
 #  UpperLimit : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

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
 

 
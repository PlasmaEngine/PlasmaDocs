 `Component` `Physics`



(NOTE) A relative velocity joint defines what the desired relative velocity on three world axes should be between two objects. Relative velocity is defined as v2 - v1. This joint has not been tested with motors or limits in any way.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#getaxis-plasma-engine-docu)| |[joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)| |
|[ GetAxisActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#getaxisactive-plasma-engin)| | | |
|[ GetMaxImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#getmaximpulse-plasma-engin)| | | |
|[ GetSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#getspeed-plasma-engine-doc)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#relativevelocityjoint-vo)| | | |
|[ SetAxis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#setaxis-void)| | | |
|[ SetAxisActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#setaxisactive-void)| | | |
|[ SetMaxImpulse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#setmaximpulse-void)| | | |
|[ SetSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjoint.md#setspeed-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  GetAxis : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> One of 3 axes to constrain movement on.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetAxis(index : Integer) : Real3
> ``` 


---  
 #  GetAxisActive : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not the given axis index is active.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetAxisActive(index : Integer) : Boolean
> ``` 


---  
 #  GetMaxImpulse : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max impulse for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetMaxImpulse(index : Integer) : Real
> ``` 


---  
 #  GetSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The desired relative speed for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetSpeed(index : Integer) : Real
> ``` 


---  
 #  RelativeVelocityJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RelativeVelocityJoint()
> ``` 


---  
 #  SetAxis : Void

> One of 3 axes to constrain movement on.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |axis|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function SetAxis(index : Integer, axis : Real3)
> ``` 


---  
 #  SetAxisActive : Void

> Whether or not the given axis index is active.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |active|[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function SetAxisActive(index : Integer, active : Boolean)
> ``` 


---  
 #  SetMaxImpulse : Void

> The max impulse for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |maxImpulse|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetMaxImpulse(index : Integer, maxImpulse : Real)
> ``` 


---  
 #  SetSpeed : Void

> The desired relative speed for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |speed|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetSpeed(index : Integer, speed : Real)
> ``` 


---  
 

 
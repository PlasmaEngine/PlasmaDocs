 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#clone-plasma-engine-docume)|[ CollapseToPoseOnFinish](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#collapsetoposeonfinish-z)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)|[basicanimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicanimation.md)|
|[ CollapseToPose](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#collapsetopose-void)|[ Duration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#duration-plasma-engine-doc)| |[dualblendchainnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dualblendchainnode.md)|
|[ GetNormalizedTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#getnormalizedtime-plasma-e)|[ Paused](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#paused-plasma-engine-docum)| |[dualblendcrossblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dualblendcrossblend.md)|
|[ IsActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#isactive-plasma-engine-doc)|[ Time](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#time-plasma-engine-documen)| |[dualblenddirectblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dualblenddirectblend.md)|
|[ PrintNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#printnode-void)|[ TimeScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#timescale-plasma-engine-do)| |[dualblendselectivenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/dualblendselectivenode.md)|
|[ SetNormalizedTime](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md#setnormalizedtime-void)| | |[posenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/posenode.md)|


 #  Properties


---  
 #  CollapseToPoseOnFinish : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not to collapse to a pose node when finished playing.
> ``` lang=cpp, name=Lightning
> var CollapseToPoseOnFinish : Boolean


---  
 #  Duration : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The duration of the node.
> ``` lang=cpp, name=Lightning
> var Duration : Real


---  
 #  Paused : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not the node is currently paused.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Time : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The current time in the node.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  TimeScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> A scalar to dt when updating the node.
> ``` lang=cpp, name=Lightning
> var TimeScale : Real


---  
 #  Methods


---  
 #  Clone : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : AnimationNode
> ``` 


---  
 #  CollapseToPose : Void

> Collapses all children to a pose node on the next Update.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CollapseToPose()
> ``` 


---  
 #  GetNormalizedTime : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetNormalizedTime() : Real
> ``` 


---  
 #  IsActive : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsActive() : Boolean
> ``` 


---  
 #  PrintNode : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |tabs|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function PrintNode(tabs : Integer)
> ``` 


---  
 #  SetNormalizedTime : Void

> A value between [0-1].
> |Name|Type|Description|
> |---|---|---|
> |normalizedTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetNormalizedTime(normalizedTime : Real)
> ``` 


---  
 

 
 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#clone-plasma-engine-docume)|[ CollapseToPoseOnFinish](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#collapsetoposeonfinish-z)|[referencecountedeventobject](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/referencecountedeventobject.markdown)|[basicanimation](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/basicanimation.markdown)|
|[ CollapseToPose](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#collapsetopose-void)|[ Duration](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#duration-plasma-engine-doc)| |[dualblendchainnode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dualblendchainnode.markdown)|
|[ GetNormalizedTime](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#getnormalizedtime-plasma-e)|[ Paused](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#paused-plasma-engine-docum)| |[dualblendcrossblend](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dualblendcrossblend.markdown)|
|[ IsActive](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#isactive-plasma-engine-doc)|[ Time](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#time-plasma-engine-documen)| |[dualblenddirectblend](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dualblenddirectblend.markdown)|
|[ PrintNode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#printnode-void)|[ TimeScale](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#timescale-plasma-engine-do)| |[dualblendselectivenode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/dualblendselectivenode.markdown)|
|[ SetNormalizedTime](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown#setnormalizedtime-void)| | |[posenode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/posenode.markdown)|


 #  Properties


---  
 #  CollapseToPoseOnFinish : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not to collapse to a pose node when finished playing.
> ``` lang=cpp, name=Lightning
> var CollapseToPoseOnFinish : Boolean


---  
 #  Duration : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The duration of the node.
> ``` lang=cpp, name=Lightning
> var Duration : Real


---  
 #  Paused : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not the node is currently paused.
> ``` lang=cpp, name=Lightning
> var Paused : Boolean


---  
 #  Time : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The current time in the node.
> ``` lang=cpp, name=Lightning
> var Time : Real


---  
 #  TimeScale : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> A scalar to dt when updating the node.
> ``` lang=cpp, name=Lightning
> var TimeScale : Real


---  
 #  Methods


---  
 #  Clone : [animationnode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/animationnode.markdown)

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
 #  GetNormalizedTime : [real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GetNormalizedTime() : Real
> ``` 


---  
 #  IsActive : [boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

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
> |tabs|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function PrintNode(tabs : Integer)
> ``` 


---  
 #  SetNormalizedTime : Void

> A value between [0-1].
> |Name|Type|Description|
> |---|---|---|
> |normalizedTime|[real](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetNormalizedTime(normalizedTime : Real)
> ``` 


---  
 

 
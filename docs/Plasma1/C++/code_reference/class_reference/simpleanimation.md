 `Component` `Engine`



(NOTE) Plays a single animation on Initialize.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ChainAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#chainanimation-plasma-engi)|[ Animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#animation-plasma-engine-do)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ CrossBlend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#crossblend-plasma-engine-d)|[ PlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#playmode-plasma-engine-doc)| | |
|[ DirectBlend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#directblend-plasma-engine)| | | |
|[ PlayIsolatedAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#playisolatedanimation-ze)| | | |
|[ PlaySingle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#playsingle-plasma-engine-d)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.md#simpleanimation-void)| | | |


 #  Properties


---  
 #  Animation : [animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)

> Animation getter/setter.
> ``` lang=cpp, name=Lightning
> var Animation : Animation


---  
 #  PlayMode : [AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)

> Play mode getter/setter.
> ``` lang=cpp, name=Lightning
> var PlayMode : AnimationPlayMode


---  
 #  Methods


---  
 #  ChainAnimation : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function ChainAnimation(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  CrossBlend : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |transitionTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function CrossBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  DirectBlend : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |transitionTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function DirectBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlayIsolatedAnimation : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |rootBone|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function PlayIsolatedAnimation(animation : Animation, rootBone : Cog, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlaySingle : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> Play animations directly.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function PlaySingle(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  SimpleAnimation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SimpleAnimation()
> ``` 


---  
 

 
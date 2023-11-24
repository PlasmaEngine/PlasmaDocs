 `Component` `Engine`



(NOTE) Plays a single animation on Initialize.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ChainAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#chainanimation-plasma-engi)|[ Animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#animation-plasma-engine-do)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
|[ CrossBlend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#crossblend-plasma-engine-d)|[ PlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#playmode-plasma-engine-doc)| | |
|[ DirectBlend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#directblend-plasma-engine)| | | |
|[ PlayIsolatedAnimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#playisolatedanimation-ze)| | | |
|[ PlaySingle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#playsingle-plasma-engine-d)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/simpleanimation.markdown#simpleanimation-void)| | | |


 #  Properties


---  
 #  Animation : [animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)

> Animation getter/setter.
> ``` lang=cpp, name=Lightning
> var Animation : Animation


---  
 #  PlayMode : [AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)

> Play mode getter/setter.
> ``` lang=cpp, name=Lightning
> var PlayMode : AnimationPlayMode


---  
 #  Methods


---  
 #  ChainAnimation : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function ChainAnimation(animation : Animation, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  CrossBlend : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |transitionTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function CrossBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  DirectBlend : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |transitionTime|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function DirectBlend(animation : Animation, transitionTime : Real, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlayIsolatedAnimation : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |rootBone|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function PlayIsolatedAnimation(animation : Animation, rootBone : Cog, playMode : AnimationPlayMode) : AnimationNode
> ``` 


---  
 #  PlaySingle : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> Play animations directly.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |playMode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
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
 

 
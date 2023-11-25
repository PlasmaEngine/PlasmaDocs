 `Component` `Engine`



(NOTE) The AnimationGraph component controls animation for an individual game object. It stores all needed per instance (vs what is shared in the animation resource) manages the current time and enumerates the animation sets. The AnimationGraph can animate multiple child objects and properties enabling bone animation, and other hierarchical animations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#animationgraph-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ CreateBasicNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#createbasicnode-plasma-eng)|[ ActiveNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#activenode-plasma-engine-d)| | |
|[ CreateChainNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#createchainnode-plasma-eng)|[ TimeScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#timescale-plasma-engine-do)| | |
|[ CreateCrossBlendNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#createcrossblendnode-zer)| | | |
|[ CreateDirectBlendNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#createdirectblendnode-ze)| | | |
|[ CreateSelectiveNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#createselectivenode-plasma)| | | |
|[ IsPlayingInGraph](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#isplayingingraph-plasma-en)| | | |
|[ PrintGraph](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#printgraph-void)| | | |
|[ Update](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.md#update-void)| | | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the animGraph animating?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  ActiveNode : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.md)

> The current root animation node.
> ``` lang=cpp, name=Lightning
> var ActiveNode : AnimationNode


---  
 #  TimeScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> A scalar to the entire animation graph.
> ``` lang=cpp, name=Lightning
> var TimeScale : Real


---  
 #  Methods


---  
 #  AnimationGraph : Void

 `constructor`

> Constructor / destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AnimationGraph()
> ``` 


---  
 #  CreateBasicNode : [basicanimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicanimation.md)

> Node creation functions.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> |mode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function CreateBasicNode(animation : Animation, mode : AnimationPlayMode) : BasicAnimation
> ``` 


---  
 #  CreateChainNode : [chainnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/chainnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateChainNode() : ChainNode
> ``` 


---  
 #  CreateCrossBlendNode : [crossblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/crossblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateCrossBlendNode() : CrossBlend
> ``` 


---  
 #  CreateDirectBlendNode : [directblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/directblend.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateDirectBlendNode() : DirectBlend
> ``` 


---  
 #  CreateSelectiveNode : [selectivenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selectivenode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateSelectiveNode() : SelectiveNode
> ``` 


---  
 #  IsPlayingInGraph : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.md)| |
> ``` lang=cpp, name=Lightning
> function IsPlayingInGraph(animation : Animation) : Boolean
> ``` 


---  
 #  PrintGraph : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PrintGraph()
> ``` 


---  
 #  Update : Void

> Updates the root node on each from and applies it to the object tree.
> |Name|Type|Description|
> |---|---|---|
> |dt|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function Update(dt : Real)
> ``` 


---  
 

 
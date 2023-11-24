 `Component` `Engine`



(NOTE) The AnimationGraph component controls animation for an individual game object. It stores all needed per instance (vs what is shared in the animation resource) manages the current time and enumerates the animation sets. The AnimationGraph can animate multiple child objects and properties enabling bone animation, and other hierarchical animations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#animationgraph-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.markdown)| |
|[ CreateBasicNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#createbasicnode-plasma-eng)|[ ActiveNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#activenode-plasma-engine-d)| | |
|[ CreateChainNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#createchainnode-plasma-eng)|[ TimeScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#timescale-plasma-engine-do)| | |
|[ CreateCrossBlendNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#createcrossblendnode-zer)| | | |
|[ CreateDirectBlendNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#createdirectblendnode-ze)| | | |
|[ CreateSelectiveNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#createselectivenode-plasma)| | | |
|[ IsPlayingInGraph](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#isplayingingraph-plasma-en)| | | |
|[ PrintGraph](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#printgraph-void)| | | |
|[ Update](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationgraph.markdown#update-void)| | | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Is the animGraph animating?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  ActiveNode : [animationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animationnode.markdown)

> The current root animation node.
> ``` lang=cpp, name=Lightning
> var ActiveNode : AnimationNode


---  
 #  TimeScale : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

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
 #  CreateBasicNode : [basicanimation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basicanimation.markdown)

> Node creation functions.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
> |mode|[AnimationPlayMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function CreateBasicNode(animation : Animation, mode : AnimationPlayMode) : BasicAnimation
> ``` 


---  
 #  CreateChainNode : [chainnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/chainnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateChainNode() : ChainNode
> ``` 


---  
 #  CreateCrossBlendNode : [crossblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/crossblend.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateCrossBlendNode() : CrossBlend
> ``` 


---  
 #  CreateDirectBlendNode : [directblend](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/directblend.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateDirectBlendNode() : DirectBlend
> ``` 


---  
 #  CreateSelectiveNode : [selectivenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/selectivenode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateSelectiveNode() : SelectiveNode
> ``` 


---  
 #  IsPlayingInGraph : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/animation.markdown)| |
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
> |dt|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Update(dt : Real)
> ``` 


---  
 

 
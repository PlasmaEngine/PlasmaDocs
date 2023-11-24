 `Component` `Engine`



(NOTE) The AnimationGraph component controls animation for an individual game object. It stores all needed per instance (vs what is shared in the animation resource) manages the current time and enumerates the animation sets. The AnimationGraph can animate multiple child objects and properties enabling bone animation, and other hierarchical animations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#animationgraph-void)|[ Active](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#active-plasma-engine-docum)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |
|[ CreateBasicNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#createbasicnode-plasma-eng)|[ ActiveNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#activenode-plasma-engine-d)| | |
|[ CreateChainNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#createchainnode-plasma-eng)|[ TimeScale](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#timescale-plasma-engine-do)| | |
|[ CreateCrossBlendNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#createcrossblendnode-zer)| | | |
|[ CreateDirectBlendNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#createdirectblendnode-ze)| | | |
|[ CreateSelectiveNode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#createselectivenode-plasma)| | | |
|[ IsPlayingInGraph](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#isplayingingraph-plasma-en)| | | |
|[ PrintGraph](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#printgraph-void)| | | |
|[ Update](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationgraph.markdown#update-void)| | | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Is the animGraph animating?
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  ActiveNode : [animationnode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animationnode.markdown)

> The current root animation node.
> ``` lang=cpp, name=Lightning
> var ActiveNode : AnimationNode


---  
 #  TimeScale : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

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
 #  CreateBasicNode : [basicanimation](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/basicanimation.markdown)

> Node creation functions.
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animation.markdown)| |
> |mode|[AnimationPlayMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#animationplaymode)| |
> ``` lang=cpp, name=Lightning
> function CreateBasicNode(animation : Animation, mode : AnimationPlayMode) : BasicAnimation
> ``` 


---  
 #  CreateChainNode : [chainnode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/chainnode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateChainNode() : ChainNode
> ``` 


---  
 #  CreateCrossBlendNode : [crossblend](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/crossblend.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateCrossBlendNode() : CrossBlend
> ``` 


---  
 #  CreateDirectBlendNode : [directblend](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/directblend.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateDirectBlendNode() : DirectBlend
> ``` 


---  
 #  CreateSelectiveNode : [selectivenode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/selectivenode.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CreateSelectiveNode() : SelectiveNode
> ``` 


---  
 #  IsPlayingInGraph : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |animation|[animation](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/animation.markdown)| |
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
> |dt|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Update(dt : Real)
> ``` 


---  
 

 
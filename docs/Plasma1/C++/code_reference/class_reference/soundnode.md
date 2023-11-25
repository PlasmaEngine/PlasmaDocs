 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddInputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#addinputnode-void)|[ AutoCollapse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#autocollapse-plasma-engine)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)|[additivesynthnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.md)|
|[ InsertNodeAfter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#insertnodeafter-void)|[ BypassPercent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#bypasspercent-plasma-engin)| |[addnoisenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/addnoisenode.md)|
|[ InsertNodeBefore](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#insertnodebefore-void)|[ BypassValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#bypassvalue-plasma-engine)| |[bandpassnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/bandpassnode.md)|
|[ RemoveAllInputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#removeallinputs-void)|[ HasInputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#hasinputs-plasma-engine-do)| |[chorusnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/chorusnode.md)|
|[ RemoveAllOutputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#removealloutputs-void)|[ HasOutputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#hasoutputs-plasma-engine-d)| |[compressornode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/compressornode.md)|
|[ RemoveAndAttachInputsToOutputs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#removeandattachinputstoo)|[ InputCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#inputcount-plasma-engine-d)| |[customaudionode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customaudionode.md)|
|[ RemoveInputNode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#removeinputnode-void)|[ OutputCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#outputcount-plasma-engine)| |[delaynode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/delaynode.md)|
|[ ReplaceWith](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md#replacewith-void)| | |[equalizernode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/equalizernode.md)|
| | | |[expandernode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/expandernode.md)|
| | | |[flangernode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/flangernode.md)|
| | | |[generatedwavenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/generatedwavenode.md)|
| | | |[granularsynthnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/granularsynthnode.md)|
| | | |[highpassnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/highpassnode.md)|
| | | |[lowpassnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/lowpassnode.md)|
| | | |[microphoneinputnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/microphoneinputnode.md)|
| | | |[modulationnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/modulationnode.md)|
| | | |[panningnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/panningnode.md)|
| | | |[pitchnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pitchnode.md)|
| | | |[recordingnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/recordingnode.md)|
| | | |[reverbnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/reverbnode.md)|
| | | |[saveaudionode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/saveaudionode.md)|
| | | |[volumenode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/volumenode.md)|


 #  Properties


---  
 #  AutoCollapse : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If true, this node will automatically remove itself from the graph when its last input node is removed.
> ``` lang=cpp, name=Lightning
> var AutoCollapse : Boolean


---  
 #  BypassPercent : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> DEPRECATED The BypassValue property should be used instead.
> ``` lang=cpp, name=Lightning
> var BypassPercent : Real


---  
 #  BypassValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The percentage of output (0 to 1.0) that should skip whatever processing the node does.
> ``` lang=cpp, name=Lightning
> var BypassValue : Real


---  
 #  HasInputs : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Will be true if this node has any input nodes.
> ``` lang=cpp, name=Lightning
> var HasInputs : Boolean


---  
 #  HasOutputs : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Will be true if this node has any output nodes.
> ``` lang=cpp, name=Lightning
> var HasOutputs : Boolean


---  
 #  InputCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The number of input nodes that are currently attached to this node.
> ``` lang=cpp, name=Lightning
> var InputCount : Integer


---  
 #  OutputCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The number of output nodes that are currently attached to this node.
> ``` lang=cpp, name=Lightning
> var OutputCount : Integer


---  
 #  Methods


---  
 #  AddInputNode : Void

> Adds the passed in node to this node's inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> ``` lang=cpp, name=Lightning
> function AddInputNode(node : SoundNode)
> ``` 


---  
 #  InsertNodeAfter : Void

> Inserts the passed in node after this node in the signal path, placing it between this node and any nodes which were connected to this node's output.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> ``` lang=cpp, name=Lightning
> function InsertNodeAfter(node : SoundNode)
> ``` 


---  
 #  InsertNodeBefore : Void

> Inserts the passed in node before this node in the signal path, placing it between this node and any nodes which were connected to this node as inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> ``` lang=cpp, name=Lightning
> function InsertNodeBefore(node : SoundNode)
> ``` 


---  
 #  RemoveAllInputs : Void

> Removes the connections between this node and all of its input nodes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RemoveAllInputs()
> ``` 


---  
 #  RemoveAllOutputs : Void

> Removes the connections between this node and all of its output nodes, disconnecting this node from the graph. If this node has no inputs it will be deleted when no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RemoveAllOutputs()
> ``` 


---  
 #  RemoveAndAttachInputsToOutputs : Void

> Removes this node from the graph by disconnecting it from all inputs and outputs and attaching the input nodes to the output nodes, keeping the rest of the graph intact. This node will be deleted when it is no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RemoveAndAttachInputsToOutputs()
> ``` 


---  
 #  RemoveInputNode : Void

> Removes the node passed in as a parameter from this node's inputs.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveInputNode(node : SoundNode)
> ``` 


---  
 #  ReplaceWith : Void

> Replaces this node in the graph with the node passed in as a parameter. This node will be deleted when it is no longer referenced.
> |Name|Type|Description|
> |---|---|---|
> |node|[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.md)| |
> ``` lang=cpp, name=Lightning
> function ReplaceWith(node : SoundNode)
> ``` 


---  
 

 
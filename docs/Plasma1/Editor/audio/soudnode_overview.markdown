# Sound Node Overview
[ SoundNodes ](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundnode.markdown) are the building blocks behind all audio in the Plasma Engine. A SoundNode receives audio data from other SoundNodes through its input connections, modifies that data in some way (or simply collects it), then passes it along to more SoundNodes through its output connections.

Some SoundNodes only generate audio data, like [SoundInstances](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundinstance.markdown). Those nodes do not collect anything from their input connections and attaching nodes to their input would have no effect.

All sound objects in the Plasma Engine use some type of SoundNode. These nodes are connected together into a tree-like graph, with generating nodes as the topmost branches, and the output node of the [SoundSpace ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundspace.markdown) as the root node at the bottom. The SoundNode graph processes audio by starting at the root node and requesting data from its input nodes. These nodes then request data from their inputs, and so on, until the request reaches a generating node which returns audio data that then follows the chain back down the graph. 

There are many types of SoundNodes that can only be created and added to the node graph in LightningScripts. These SoundNodes are reference counted: they will stay alive as long as the user stores a variable with the SoundNode assigned to it. If it is not stored, the node will be alive as long as it is connected to the graph, but users can no longer access it. 

The SoundNodes of built-in objects are also exposed in Lightning, and users can freely edit most of the graph connections, giving them a great deal of flexibility in creating audio. When building connections it is important to remember that nodes closer to the generating node modify the audio before nodes that are further away. For example, to change the pitch of a sound before applying reverb, the PitchNode must be between the SoundInstance and the ReverbNode. 

The [SoundNode Graph ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode_graph.markdown) tool can be extremely helpful when editing the graph directly.

WARNING: SoundNodes can be connected in many complicated ways, but users must be careful not to create a loop. If loops are created, the user will receive an error, and the SoundNodes will be automatically disconnected.

In most cases, nodes can be connected in any order and to any number of other nodes. The exception is the [PitchNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/pitchnode.markdown). The PitchNode changes the pitch of a sound by essentially stretching or squishing the sound waves, which means that it needs a different amount of data than other nodes. This causes a problem when a PitchNode and a node that was not pitch-shifted request data from the same SoundInstance.

WARNING: When using PitchNodes, if a generating node has multiple output connections the user must make sure all of them are at the same pitch. If SoundNodes request data from the generating node at different pitch settings there will be an error and the nodes will be disconnected.

# Using SoundNodes

In LightningScripts, all SoundNodes are created using the appropriate method on the Audio object. The following code block shows how you would create a PitchNode.
<pre><code class="language-csharp">
var myPitchNode = Audio.PitchNode();
</code></pre>

There are multiple places in the SoundNode Graph that sound nodes can be attached.  Here is an example of a component that creates and controls a PitchNode for its neighboring [SoundEmitter](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundemitter.markdown):
<pre><code class="language-csharp">
class EmitterPitch : LightningComponent
{
  [Dependency] var SoundEmitter : SoundEmitter;
  
  var PitchNode : PitchNode = Audio.PitchNode();
  [Property] var Pitch : Real
  {
    get { return this.PitchNode.Pitch; }
    set { this.PitchNode.Pitch = value; }
  }
  
  function Initialize(init : CogInitializer)
  {
    this.SoundEmitter.OutputNode.InsertNodeAfter(this.PitchNode);
  }
}
</code></pre>

The functionality described below is available on all SoundNodes. See the individual [Manual pages](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode.markdown) for details about each SoundNode type.

## Adding and Removing SoundNodes 

To add a SoundNode as input on another SoundNode, call the `AddInputNode` method on the SoundNode that should receive the input, passing in the input SoundNode as the parameter.

There are two ways to insert a SoundNode into the existing graph, `InsertNodeAfter` and `InsertNodeBefore`. As expected, `InsertNodeAfter` will insert a SoundNode into the graph after the SoundNode the method is called on (placing it between that SoundNode and all its output nodes), and `InsertNodeBefore` will insert a SoundNode before the SoundNode the method is called on (placing it between that SoundNode and all its input nodes).

NOTE: Some built-in objects do not allow insertion and will give a warning if the user calls this method. 

To disconnect a SoundNode's input, the `RemoveAllInputs` method can be used to remove all input connections from the SoundNode. Removing a single input can be done using the `RemoveInputNode` method, which will remove the SoundNode passed in as the parameter from the inputs of the SoundNode the method is called on. The `RemoveAllOutputs` method will remove all output connections from the SoundNode, disconnecting it from the node graph. 

There are two ways to remove a SoundNode from the graph while keeping the rest of the graph intact. The `RemoveAndAttachInputsToOutputs` method will remove the SoundNode from the graph but will also connect all of the SoundNode's input SoundNodes to all of its output SoundNodes. The `ReplaceWith` method will replace the SoundNode the method is called on with the SoundNode passed in as the parameter; all inputs and outputs of the SoundNode the method is called on will be switched to the new SoundNode.

NOTE: Built in objects that do not allow insertion before their SoundNode also do not allow you to remove all of their inputs. Built in objects such as  SoundSpaces will not allow you to remove them from the graph.

## Bypassing SoundNodes

The `BypassPercent` property sets a percentage of a SoundNode's input that will be sent directly to its outputs, without any processing. In other words, if the `BypassPercent` is set to 30.0, seventy percent of the sound will be processed by the SoundNode while thirty percent will not. This can be a useful way to turn nodes on and off without removing them from the graph, or to reduce the strength of an audio effect.

NOTE: On some types of SoundNodes changing this value by large amounts at runtime could result in clicks or other problems with the audio. 

## Collapsing Unused SoundNodes

If the `AutoCollapse` property is set to True, the SoundNode will automatically remove itself from the graph when its last input node is removed. This property is set to False by default. 

## Lightning Events

- The `SoundNodeDisconnected` [ SoundEvent ](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundevent.markdown) is sent by all SoundNodes when they are is completely disconnected from the graph (when the node has no more inputs or outputs).

# Related Materials

## Manual
- [SoundInstance ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundinstance.markdown)
- [SoundSpace ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/oundnode/soundspace.markdown)
- [SoundNode Graph ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode_graph.markdown)

 ## Reference
- [ SoundNode ](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/soundnode.markdown) 

 
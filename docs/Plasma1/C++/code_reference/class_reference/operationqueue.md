 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ BeginBatch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#beginbatch-void)|[ ActiveBatchName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#activebatchname-plasma-eng)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)| |
|[ ClearAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#clearall-void)|[ Commands](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#commands-plasma-engine-doc)| | |
|[ ClearRedo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#clearredo-void)|[ RedoCommands](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#redocommands-plasma-engine)| | |
|[ ClearUndo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#clearundo-void)| | | |
|[ DestroyObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#destroyobject-void)| | | |
|[ EndBatch](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#endbatch-void)| | | |
|[ IsListeningForSideEffects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#islisteningforsideeffect)| | | |
|[ MarkPropertyAsModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#markpropertyasmodified-v)| | | |
|[ ObjectCreated](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#objectcreated-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#operationqueue-void)| | | |
|[ PopSubPropertyContext](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#popsubpropertycontext-vo)| | | |
|[ QueueRegisteredSideEffects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#queueregisteredsideeffec)| | | |
|[ Redo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#redo-void)| | | |
|[ RegisterSideEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#registersideeffect-void)| | | |
|[ SaveObjectState](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#saveobjectstate-void)| | | |
|[ StartListeningForSideEffects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#startlisteningforsideeff)| | | |
|[ Undo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md#undo-void)| | | |


 #  Properties


---  
 #  ActiveBatchName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var ActiveBatchName : String


---  
 #  Commands : [operationlistrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationlistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Commands : OperationListRange


---  
 #  RedoCommands : [operationlistrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationlistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var RedoCommands : OperationListRange


---  
 #  Methods


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function BeginBatch()
> ``` 


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function BeginBatch(p0 : String)
> ``` 


---  
 #  ClearAll : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearAll()
> ``` 


---  
 #  ClearRedo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearRedo()
> ``` 


---  
 #  ClearUndo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearUndo()
> ``` 


---  
 #  DestroyObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function DestroyObject(p0 : Cog)
> ``` 


---  
 #  EndBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function EndBatch()
> ``` 


---  
 #  IsListeningForSideEffects : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsListeningForSideEffects() : Boolean
> ``` 


---  
 #  MarkPropertyAsModified : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
> |p1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function MarkPropertyAsModified(p0 : Component, p1 : String)
> ``` 


---  
 #  ObjectCreated : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function ObjectCreated(p0 : Cog)
> ``` 


---  
 #  OperationQueue : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function OperationQueue()
> ``` 


---  
 #  PopSubPropertyContext : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PopSubPropertyContext()
> ``` 


---  
 #  QueueRegisteredSideEffects : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function QueueRegisteredSideEffects()
> ``` 


---  
 #  Redo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Redo()
> ``` 


---  
 #  Redo : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operation.md)| |
> ``` lang=cpp, name=Lightning
> function Redo(p0 : Operation) : Boolean
> ``` 


---  
 #  RegisterSideEffect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)| |
> |p1|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |p2|T| |
> ``` lang=cpp, name=Lightning
> function RegisterSideEffect(p0 : AnyHandle, p1 : String, p2 : T)
> ``` 


---  
 #  SaveObjectState : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function SaveObjectState(p0 : Cog)
> ``` 


---  
 #  StartListeningForSideEffects : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StartListeningForSideEffects()
> ``` 


---  
 #  Undo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Undo()
> ``` 


---  
 #  Undo : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operation.md)| |
> ``` lang=cpp, name=Lightning
> function Undo(p0 : Operation) : Boolean
> ``` 


---  
 

 
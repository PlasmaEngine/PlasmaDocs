 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObject](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#addobject-void)|[ Basis](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#basis-plasma-engine-docume)|[component](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)|[objectrotategizmo](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objectrotategizmo.markdown)|
|[ ClearObjects](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#clearobjects-void)|[ ObjectCount](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#objectcount-plasma-engine)| |[objectscalegizmo](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objectscalegizmo.markdown)|
|[ GetObjectAtIndex](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#getobjectatindex-plasma-en)|[ Pivot](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#pivot-plasma-engine-docume)| |[objecttranslategizmo](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttranslategizmo.markdown)|
|[ Constructor](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#objecttransformgizmo-voi)| | | |
|[ RemoveObject](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#removeobject-void)| | | |
|[ SetOperationQueue](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#setoperationqueue-void)| | | |
|[ ToggleCoordinateMode](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/objecttransformgizmo.markdown#togglecoordinatemode-voi)| | | |


 #  Properties


---  
 #  Basis : [GizmoBasis](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#gizmobasis)

> Setters / Getters.
> ``` lang=cpp, name=Lightning
> var Basis : GizmoBasis


---  
 #  ObjectCount : [integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Object getters.
> ``` lang=cpp, name=Lightning
> var ObjectCount : Integer


---  
 #  Pivot : [GizmoPivot](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#gizmopivot)

> 
> ``` lang=cpp, name=Lightning
> var Pivot : GizmoPivot


---  
 #  Methods


---  
 #  AddObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||[anyhandle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/anyhandle.markdown)| |
> ||[boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function AddObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  ClearObjects : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearObjects()
> ``` 


---  
 #  GetObjectAtIndex : [anyhandle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/anyhandle.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetObjectAtIndex(index : Integer) : AnyHandle
> ``` 


---  
 #  ObjectTransformGizmo : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ObjectTransformGizmo()
> ``` 


---  
 #  RemoveObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||[anyhandle](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/anyhandle.markdown)| |
> ||[boolean](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)| |
> ``` lang=cpp, name=Lightning
> function RemoveObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  SetOperationQueue : Void

> If set, this Gizmo will add operations for all modifications to cogs.
> |Name|Type|Description|
> |---|---|---|
> |opQueue|[operationqueue](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/operationqueue.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetOperationQueue(opQueue : OperationQueue)
> ``` 


---  
 #  ToggleCoordinateMode : Void

> Toggle between local / world.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ToggleCoordinateMode()
> ``` 


---  
 

 
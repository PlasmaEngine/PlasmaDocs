 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#addobject-void)|[ Basis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#basis-plasma-engine-docume)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)|[objectrotategizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectrotategizmo.md)|
|[ ClearObjects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#clearobjects-void)|[ ObjectCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#objectcount-plasma-engine)| |[objectscalegizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectscalegizmo.md)|
|[ GetObjectAtIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#getobjectatindex-plasma-en)|[ Pivot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#pivot-plasma-engine-docume)| |[objecttranslategizmo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttranslategizmo.md)|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#objecttransformgizmo-voi)| | | |
|[ RemoveObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#removeobject-void)| | | |
|[ SetOperationQueue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#setoperationqueue-void)| | | |
|[ ToggleCoordinateMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objecttransformgizmo.md#togglecoordinatemode-voi)| | | |


 #  Properties


---  
 #  Basis : [GizmoBasis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#gizmobasis)

> Setters / Getters.
> ``` lang=cpp, name=Lightning
> var Basis : GizmoBasis


---  
 #  ObjectCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Object getters.
> ``` lang=cpp, name=Lightning
> var ObjectCount : Integer


---  
 #  Pivot : [GizmoPivot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#gizmopivot)

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
> ||[anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)| |
> ||[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
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
 #  GetObjectAtIndex : [anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
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
> ||[anyhandle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/anyhandle.md)| |
> ||[boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  SetOperationQueue : Void

> If set, this Gizmo will add operations for all modifications to cogs.
> |Name|Type|Description|
> |---|---|---|
> |opQueue|[operationqueue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/operationqueue.md)| |
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
 

 
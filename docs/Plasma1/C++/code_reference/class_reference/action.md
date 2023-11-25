 `Engine`

(NOTE) Base action class.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Cancel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/action.md#cancel-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/action.md#active-plasma-engine-docum)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)|[actiondelay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/actiondelay.md)|
| |[ Completed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/action.md#completed-plasma-engine-do)| |[actionset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/actionset.md)|
| |[ Started](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/action.md#started-plasma-engine-docu)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> The action is queued and not stared or running.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  Completed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> The action ran until it completed.
> ``` lang=cpp, name=Lightning
> var Completed : Boolean


---  
 #  Started : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Has the action started?
> ``` lang=cpp, name=Lightning
> var Started : Boolean


---  
 #  Methods


---  
 #  Cancel : Void

> Cancel the action and all child actions.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Cancel()
> ``` 


---  
 

 
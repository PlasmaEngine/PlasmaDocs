 `Engine`

(NOTE) Base action class.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Cancel](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/action.markdown#cancel-void)|[ Active](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/action.markdown#active-plasma-engine-docum)|[referencecountedeventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/referencecountedeventobject.markdown)|[actiondelay](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/actiondelay.markdown)|
| |[ Completed](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/action.markdown#completed-plasma-engine-do)| |[actionset](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/actionset.markdown)|
| |[ Started](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/action.markdown#started-plasma-engine-docu)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> The action is queued and not stared or running.
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  Completed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> The action ran until it completed.
> ``` lang=cpp, name=Lightning
> var Completed : Boolean


---  
 #  Started : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

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
 

 
 `Component` `Gameplay`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Capture](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousecapture.md#capture-plasma-engine-docu)|[ IsCaptured](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousecapture.md#iscaptured-plasma-engine-d)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousecapture.md#mousecapture-void)| | | |
|[ ReleaseCapture](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mousecapture.md#releasecapture-void)| | | |


 #  Properties


---  
 #  IsCaptured : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Returns whether or not this has an active mouse capture.
> ``` lang=cpp, name=Lightning
> var IsCaptured : Boolean


---  
 #  Methods


---  
 #  Capture : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Starts the mouse manipulation. All mouse events will now only go to the owner of this Component. Returns whether or not the manipulation can be started.
> |Name|Type|Description|
> |---|---|---|
> |e|[viewportmouseevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md)| |
> ``` lang=cpp, name=Lightning
> function Capture(e : ViewportMouseEvent) : Boolean
> ``` 


---  
 #  MouseCapture : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MouseCapture()
> ``` 


---  
 #  ReleaseCapture : Void

> Releases the mouse manipulation.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ReleaseCapture()
> ``` 


---  
 #  ReleaseCapture : Void

> Releases the mouse manipulation.
> |Name|Type|Description|
> |---|---|---|
> |e|[viewportmouseevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md)| |
> ``` lang=cpp, name=Lightning
> function ReleaseCapture(e : ViewportMouseEvent)
> ``` 


---  
 

 
 `Component` `Gameplay`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Capture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousecapture.markdown#capture-plasma-engine-docu)|[ IsCaptured](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousecapture.markdown#iscaptured-plasma-engine-d)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousecapture.markdown#mousecapture-void)| | | |
|[ ReleaseCapture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/mousecapture.markdown#releasecapture-void)| | | |


 #  Properties


---  
 #  IsCaptured : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Returns whether or not this has an active mouse capture.
> ``` lang=cpp, name=Lightning
> var IsCaptured : Boolean


---  
 #  Methods


---  
 #  Capture : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Starts the mouse manipulation. All mouse events will now only go to the owner of this Component. Returns whether or not the manipulation can be started.
> |Name|Type|Description|
> |---|---|---|
> |e|[viewportmouseevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/viewportmouseevent.markdown)| |
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
> |e|[viewportmouseevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/viewportmouseevent.markdown)| |
> ``` lang=cpp, name=Lightning
> function ReleaseCapture(e : ViewportMouseEvent)
> ``` 


---  
 

 
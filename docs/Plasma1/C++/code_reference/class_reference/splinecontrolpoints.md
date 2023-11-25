 `Engine`

(NOTE) Control points for the Spline class. Modifying this will cause the spline to be marked as modified to rebuild the baked curve when needed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md#add-void)|[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md#count-plasma-engine-docume)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.md)| |
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md#clear-void)| | | |
|[ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md#get-plasma-engine-document)| | | |
|[ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md#set-void)| | | |


 #  Properties


---  
 #  Count : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> The number of control points contained.
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  Methods


---  
 #  Add : Void

> Add a new point to the end of the array.
> |Name|Type|Description|
> |---|---|---|
> |controlPoint|[splinecontrolpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoint.md)| |
> ``` lang=cpp, name=Lightning
> function Add(controlPoint : SplineControlPoint)
> ``` 


---  
 #  Clear : Void

> Clear all control points.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Get : [splinecontrolpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoint.md)

> Get the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : SplineControlPoint
> ``` 


---  
 #  Set : Void

> Sets the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> |value|[splinecontrolpoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoint.md)| |
> ``` lang=cpp, name=Lightning
> function Set(index : Integer, value : SplineControlPoint)
> ``` 


---  
 

 
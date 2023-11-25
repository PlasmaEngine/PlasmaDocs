 `Component` `Engine`



(NOTE) A spline that builds its control points from all child cogs that have Transforms.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ForceRebuild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#forcerebuild-void)|[ Closed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#closed-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#hierarchyspline-void)|[ DebugDrawSpline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#debugdrawspline-plasma-eng)| | |
|[ RebuildIfModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#rebuildifmodified-void)|[ Error](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#error-plasma-engine-docume)| | |
| |[ Spline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#spline-plasma-engine-docum)| | |
| |[ SplineColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#splinecolor-plasma-engine)| | |
| |[ SplineType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchyspline.md#splinetype-plasma-engine-d)| | |


 #  Properties


---  
 #  Closed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Does the spline loop back on itself?
> ``` lang=cpp, name=Lightning
> var Closed : Boolean


---  
 #  DebugDrawSpline : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the spline draw every frame? Mainly used for debugging purposes.
> ``` lang=cpp, name=Lightning
> var DebugDrawSpline : Boolean


---  
 #  Error : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ``` lang=cpp, name=Lightning
> var Error : Real


---  
 #  Spline : [spline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md)

 `read-only`

> The internal spline data.
> ``` lang=cpp, name=Lightning
> var Spline : Spline


---  
 #  SplineColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> What color should that spline be drawn with.
> ``` lang=cpp, name=Lightning
> var SplineColor : Real4


---  
 #  SplineType : [SplineType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ``` lang=cpp, name=Lightning
> var SplineType : SplineType


---  
 #  Methods


---  
 #  ForceRebuild : Void

> Forcibly rebuilds the baked points for the spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ForceRebuild()
> ``` 


---  
 #  HierarchySpline : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function HierarchySpline()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points if there are any changes to the spline's control points. This should never need to be manually called.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RebuildIfModified()
> ``` 


---  
 

 
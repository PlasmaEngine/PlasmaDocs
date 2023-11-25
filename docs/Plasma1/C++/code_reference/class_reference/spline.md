 `Engine`

(NOTE) A spline built from control points. Bakes out the curve using an error term (distance from actual spline). Provides an interface to sample the curve at a given arc-length distance in order to provide constant speed interpolation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#clone-plasma-engine-docume)|[ BakedPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#bakedpoints-plasma-engine)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)| |
|[ Create](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#create-plasma-engine-docum)|[ Closed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#closed-plasma-engine-docum)| | |
|[ DebugDraw](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#debugdraw-void)|[ ControlPoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#controlpoints-plasma-engin)| | |
|[ ForceRebuild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#forcerebuild-void)|[ Error](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#error-plasma-engine-docume)| | |
|[ RebuildIfModified](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#rebuildifmodified-void)|[ SplineType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#splinetype-plasma-engine-d)| | |
|[ SampleDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#sampledistance-plasma-engi)|[ TotalDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#totaldistance-plasma-engin)| | |
|[ SampleNormalized](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md#samplenormalized-plasma-en)| | | |


 #  Properties


---  
 #  BakedPoints : [splinebakedpoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinebakedpoints.md)

 `read-only`

> The read-only curve points baked out to line segments using the provided error.
> ``` lang=cpp, name=Lightning
> var BakedPoints : SplineBakedPoints


---  
 #  Closed : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Does the spline loop back on itself?
> ``` lang=cpp, name=Lightning
> var Closed : Boolean


---  
 #  ControlPoints : [splinecontrolpoints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinecontrolpoints.md)

 `read-only`

> The control points used to bake out the curve.
> ``` lang=cpp, name=Lightning
> var ControlPoints : SplineControlPoints


---  
 #  Error : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ``` lang=cpp, name=Lightning
> var Error : Real


---  
 #  SplineType : [SplineType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ``` lang=cpp, name=Lightning
> var SplineType : SplineType


---  
 #  TotalDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> The total arc-length of the curve. Use to normalize the curve if you wish.
> ``` lang=cpp, name=Lightning
> var TotalDistance : Real


---  
 #  Methods


---  
 #  Clone : [spline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md)

> Create a new copy of this spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : Spline
> ``` 


---  
 #  Create : [spline](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spline.md)

 `static`

> Create a new instance of a spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Create() : Spline
> ``` 


---  
 #  DebugDraw : Void

> Draw the baked points of the curve with the provided color.
> |Name|Type|Description|
> |---|---|---|
> |color|[real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)| |
> ``` lang=cpp, name=Lightning
> function DebugDraw(color : Real4)
> ``` 


---  
 #  ForceRebuild : Void

> Forcibly rebuild the baked points from the control points.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ForceRebuild()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points from the control points if they have changed. Should not need to be manually called unless the user wants to control the timing when the points are baked.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RebuildIfModified()
> ``` 


---  
 #  SampleDistance : [splinesampledata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinesampledata.md)

> Samples the curve at a given arc-length distance.
> |Name|Type|Description|
> |---|---|---|
> |distance|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SampleDistance(distance : Real) : SplineSampleData
> ``` 


---  
 #  SampleNormalized : [splinesampledata](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/splinesampledata.md)

> Samples the curve with a time in the range of [0, 1].
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SampleNormalized(time : Real) : SplineSampleData
> ``` 


---  
 

 
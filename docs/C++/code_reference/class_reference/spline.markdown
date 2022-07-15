 `Engine`

(NOTE) A spline built from control points. Bakes out the curve using an error term (distance from actual spline). Provides an interface to sample the curve at a given arc-length distance in order to provide constant speed interpolation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#clone-plasma-engine-docume)|[ BakedPoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#bakedpoints-plasma-engine)|[referencecountedeventobject](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/referencecountedeventobject.markdown)| |
|[ Create](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#create-plasma-engine-docum)|[ Closed](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#closed-plasma-engine-docum)| | |
|[ DebugDraw](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#debugdraw-void)|[ ControlPoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#controlpoints-plasma-engin)| | |
|[ ForceRebuild](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#forcerebuild-void)|[ Error](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#error-plasma-engine-docume)| | |
|[ RebuildIfModified](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#rebuildifmodified-void)|[ SplineType](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#splinetype-plasma-engine-d)| | |
|[ SampleDistance](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#sampledistance-plasma-engi)|[ TotalDistance](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#totaldistance-plasma-engin)| | |
|[ SampleNormalized](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown#samplenormalized-plasma-en)| | | |


 #  Properties


---  
 #  BakedPoints : [splinebakedpoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/splinebakedpoints.markdown)

 `read-only`

> The read-only curve points baked out to line segments using the provided error.
> ``` lang=cpp, name=Lightning
> var BakedPoints : SplineBakedPoints


---  
 #  Closed : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Does the spline loop back on itself?
> ``` lang=cpp, name=Lightning
> var Closed : Boolean


---  
 #  ControlPoints : [splinecontrolpoints](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/splinecontrolpoints.markdown)

 `read-only`

> The control points used to bake out the curve.
> ``` lang=cpp, name=Lightning
> var ControlPoints : SplineControlPoints


---  
 #  Error : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The max number of units that a line segment is allowed to deviate from the curve.
> ``` lang=cpp, name=Lightning
> var Error : Real


---  
 #  SplineType : [SplineType](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ``` lang=cpp, name=Lightning
> var SplineType : SplineType


---  
 #  TotalDistance : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

 `read-only`

> The total arc-length of the curve. Use to normalize the curve if you wish.
> ``` lang=cpp, name=Lightning
> var TotalDistance : Real


---  
 #  Methods


---  
 #  Clone : [spline](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown)

> Create a new copy of this spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : Spline
> ``` 


---  
 #  Create : [spline](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spline.markdown)

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
> |color|[real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)| |
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
 #  SampleDistance : [splinesampledata](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/splinesampledata.markdown)

> Samples the curve at a given arc-length distance.
> |Name|Type|Description|
> |---|---|---|
> |distance|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SampleDistance(distance : Real) : SplineSampleData
> ``` 


---  
 #  SampleNormalized : [splinesampledata](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/splinesampledata.markdown)

> Samples the curve with a time in the range of [0, 1].
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SampleNormalized(time : Real) : SplineSampleData
> ``` 


---  
 

 
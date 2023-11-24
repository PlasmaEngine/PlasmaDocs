 `Event` `Gameplay`



(NOTE) All mouse events that are forwarded to reactive components or the space use this event to add extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ToWorldPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#toworldplane-plasma-engine)|[ CameraViewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#cameraviewport-plasma-engi)|[mouseevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.markdown)|[manipulatortoolevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatortoolevent.markdown)|
|[ ToWorldViewPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#toworldviewplane-plasma-en)|[ HitDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#hitdistance-plasma-engine)| | |
|[ ToWorldZPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#toworldzplane-plasma-engin)|[ HitNormal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#hitnormal-plasma-engine-do)| | |
| |[ HitObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#hitobject-plasma-engine-do)| | |
| |[ HitPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#hitposition-plasma-engine)| | |
| |[ HitUv](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#hituv-plasma-engine-docume)| | |
| |[ RayDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#raydirection-plasma-engine)| | |
| |[ RayStart](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#raystart-plasma-engine-doc)| | |
| |[ WorldRay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.markdown#worldray-plasma-engine-doc)| | |


 #  Properties


---  
 #  CameraViewport : [cameraviewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.markdown)

 `read-only`

> Camera viewport that generated this event.
> ``` lang=cpp, name=Lightning
> var CameraViewport : CameraViewport


---  
 #  HitDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The distance away the hit point is. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitDistance : Real


---  
 #  HitNormal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The normal at the intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitNormal : Real3


---  
 #  HitObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.markdown)

 `read-only`

> Object hit in ray cast.
> ``` lang=cpp, name=Lightning
> var HitObject : Cog


---  
 #  HitPosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitPosition : Real3


---  
 #  HitUv : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

> The uv texture coordinate at the intersection point, if applicable. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitUv : Real2


---  
 #  RayDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Mouse Ray Direction.
> ``` lang=cpp, name=Lightning
> var RayDirection : Real3


---  
 #  RayStart : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Mouse Ray start.
> ``` lang=cpp, name=Lightning
> var RayStart : Real3


---  
 #  WorldRay : [ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.markdown)

> The world mouse ray.
> ``` lang=cpp, name=Lightning
> var WorldRay : Ray


---  
 #  Methods


---  
 #  ToWorldPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The world mouse position on any arbitrary plane.
> |Name|Type|Description|
> |---|---|---|
> |worldPlaneNormal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> |worldPlanePosition|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function ToWorldPlane(worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ToWorldViewPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The world mouse position on the view plane at view depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function ToWorldViewPlane(viewDepth : Real) : Real3
> ``` 


---  
 #  ToWorldZPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> The world mouse position on the z plane at depth.
> |Name|Type|Description|
> |---|---|---|
> |worldDepth|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function ToWorldZPlane(worldDepth : Real) : Real3
> ``` 


---  
 

 
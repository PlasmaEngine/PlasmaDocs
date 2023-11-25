 `Event` `Gameplay`



(NOTE) All mouse events that are forwarded to reactive components or the space use this event to add extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ToWorldPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#toworldplane-plasma-engine)|[ CameraViewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#cameraviewport-plasma-engi)|[mouseevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouseevent.md)|[manipulatortoolevent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatortoolevent.md)|
|[ ToWorldViewPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#toworldviewplane-plasma-en)|[ HitDistance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#hitdistance-plasma-engine)| | |
|[ ToWorldZPlane](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#toworldzplane-plasma-engin)|[ HitNormal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#hitnormal-plasma-engine-do)| | |
| |[ HitObject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#hitobject-plasma-engine-do)| | |
| |[ HitPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#hitposition-plasma-engine)| | |
| |[ HitUv](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#hituv-plasma-engine-docume)| | |
| |[ RayDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#raydirection-plasma-engine)| | |
| |[ RayStart](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#raystart-plasma-engine-doc)| | |
| |[ WorldRay](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md#worldray-plasma-engine-doc)| | |


 #  Properties


---  
 #  CameraViewport : [cameraviewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.md)

 `read-only`

> Camera viewport that generated this event.
> ``` lang=cpp, name=Lightning
> var CameraViewport : CameraViewport


---  
 #  HitDistance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The distance away the hit point is. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitDistance : Real


---  
 #  HitNormal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The normal at the intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitNormal : Real3


---  
 #  HitObject : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> Object hit in ray cast.
> ``` lang=cpp, name=Lightning
> var HitObject : Cog


---  
 #  HitPosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitPosition : Real3


---  
 #  HitUv : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> The uv texture coordinate at the intersection point, if applicable. Used with Reactive components.
> ``` lang=cpp, name=Lightning
> var HitUv : Real2


---  
 #  RayDirection : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Mouse Ray Direction.
> ``` lang=cpp, name=Lightning
> var RayDirection : Real3


---  
 #  RayStart : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Mouse Ray start.
> ``` lang=cpp, name=Lightning
> var RayStart : Real3


---  
 #  WorldRay : [ray](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/ray.md)

> The world mouse ray.
> ``` lang=cpp, name=Lightning
> var WorldRay : Ray


---  
 #  Methods


---  
 #  ToWorldPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The world mouse position on any arbitrary plane.
> |Name|Type|Description|
> |---|---|---|
> |worldPlaneNormal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |worldPlanePosition|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function ToWorldPlane(worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ToWorldViewPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The world mouse position on the view plane at view depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function ToWorldViewPlane(viewDepth : Real) : Real3
> ``` 


---  
 #  ToWorldZPlane : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The world mouse position on the z plane at depth.
> |Name|Type|Description|
> |---|---|---|
> |worldDepth|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function ToWorldZPlane(worldDepth : Real) : Real3
> ``` 


---  
 

 
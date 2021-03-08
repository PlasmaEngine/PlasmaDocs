 `Component` `Graphics`



(NOTE) Represents a viewpoint for rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#camera-void)|[ CameraViewportCog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#cameraviewportcog-plasma-e)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ GetFrustum](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#getfrustum-plasma-engine-d)|[ FarPlane](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#farplane-plasma-engine-doc)| | |
| |[ FieldOfView](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#fieldofview-plasma-engine)| | |
| |[ NearPlane](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#nearplane-plasma-engine-do)| | |
| |[ PerspectiveMode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#perspectivemode-plasma-eng)| | |
| |[ Size](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#size-plasma-engine-documen)| | |
| |[ WorldDirection](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#worlddirection-plasma-engi)| | |
| |[ WorldTranslation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#worldtranslation-plasma-en)| | |
| |[ WorldUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown#worldup-plasma-engine-docu)| | |


 #  Properties


---  
 #  CameraViewportCog : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

 `read-only`

> The object that has a CameraViewport component using this Camera, if any.
> ``` lang=cpp, name=Lightning
> var CameraViewportCog : Cog


---  
 #  FarPlane : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The far clipping plane, always positive and in the view direction.
> ``` lang=cpp, name=Lightning
> var FarPlane : Real


---  
 #  FieldOfView : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The vertical field of view of the Camera, in degrees. Horizontal fov derived from aspect ratio (Hor+).
> ``` lang=cpp, name=Lightning
> var FieldOfView : Real


---  
 #  NearPlane : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> The near clipping plane, always positive and in the view direction.
> ``` lang=cpp, name=Lightning
> var NearPlane : Real


---  
 #  PerspectiveMode : [PerspectiveMode](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#perspectivemode)

> How the scene is projected on to the view plane.
> ``` lang=cpp, name=Lightning
> var PerspectiveMode : PerspectiveMode


---  
 #  Size : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Size (width and height) of the orthographic projection, in world units.
> ``` lang=cpp, name=Lightning
> var Size : Real


---  
 #  WorldDirection : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> Direction the Camera is facing, in world space.
> ``` lang=cpp, name=Lightning
> var WorldDirection : Real3


---  
 #  WorldTranslation : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> Translation of the Camera, in world space.
> ``` lang=cpp, name=Lightning
> var WorldTranslation : Real3


---  
 #  WorldUp : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The upright direction of the Camera(perpendicular to facing direction), in world space.
> ``` lang=cpp, name=Lightning
> var WorldUp : Real3


---  
 #  Methods


---  
 #  Camera : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Camera()
> ``` 


---  
 #  GetFrustum : [frustum](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/frustum.markdown)

> Creates a frustum using the Camera's settings along with the given aspect ratio.
> |Name|Type|Description|
> |---|---|---|
> |aspect|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetFrustum(aspect : Real) : Frustum
> ``` 


---  
 

 
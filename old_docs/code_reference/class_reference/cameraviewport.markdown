 `Component` `Gameplay`



(NOTE) Manages all setup between Camera, Renderer, and viewport UI that is required to define how anything is to be rendered.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#cameraviewport-void)|[ Camera](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#camera-plasma-engine-docum)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ ScreenToViewport](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#screentoviewport-plasma-en)|[ CameraPath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#camerapath-plasma-engine-d)| | |
|[ ScreenToWorldPlane](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#screentoworldplane-plasma)|[ FinalTexture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#finaltexture-plasma-engine)| | |
|[ ScreenToWorldRay](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#screentoworldray-plasma-en)|[ ForwardViewportEvents](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#forwardviewportevents-ze)| | |
|[ ScreenToWorldViewPlane](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#screentoworldviewplane-z)|[ Frustum](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#frustum-plasma-engine-docu)| | |
|[ ScreenToWorldZPlane](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#screentoworldzplane-plasma)|[ MarginColor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#margincolor-plasma-engine)| | |
|[ ViewPlaneSize](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewplanesize-plasma-engin)|[ MouseWorldRay](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#mouseworldray-plasma-engin)| | |
|[ ViewportTakeFocus](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewporttakefocus-plasma-e)|[ NormalizedOffset](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#normalizedoffset-plasma-en)| | |
|[ ViewportToScreen](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewporttoscreen-plasma-en)|[ NormalizedSize](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#normalizedsize-plasma-engi)| | |
|[ WorldToScreen](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#worldtoscreen-plasma-engin)|[ RendererPath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#rendererpath-plasma-engine)| | |
| |[ RenderInEditor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#renderineditor-plasma-engi)| | |
| |[ RenderInGame](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#renderingame-plasma-engine)| | |
| |[ RenderOrder](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#renderorder-plasma-engine)| | |
| |[ RenderToViewport](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#rendertoviewport-plasma-en)| | |
| |[ ResolutionOrAspect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#resolutionoraspect-plasma)| | |
| |[ ViewportHasFocus](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewporthasfocus-plasma-en)| | |
| |[ ViewportOffset](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewportoffset-plasma-engi)| | |
| |[ ViewportOffsetWithMargin](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewportoffsetwithmargin)| | |
| |[ ViewportResolution](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewportresolution-plasma)| | |
| |[ ViewportResolutionWithMargin](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewportresolutionwithma)| | |
| |[ ViewportScaling](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewportscaling-plasma-eng)| | |
| |[ ViewToPerspective](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#viewtoperspective-plasma-e)| | |
| |[ WorldToPerspective](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#worldtoperspective-plasma)| | |
| |[ WorldToView](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cameraviewport.markdown#worldtoview-plasma-engine)| | |


 #  Properties


---  
 #  Camera : [camera](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/camera.markdown)

 `read-only`

> Find the Camera component from the CameraPath (or null if it doesn't exist).
> ``` lang=cpp, name=Lightning
> var Camera : Camera


---  
 #  CameraPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cogpath.markdown)

> Object with the Camera component to be used for rendering. A Camera can only be used by one CameraViewport, if already used by another usage will be stolen when assigned.
> ``` lang=cpp, name=Lightning
> var CameraPath : CogPath


---  
 #  FinalTexture : [texture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/texture.markdown)

 `read-only`

> Texture that contains the end result of this CameraViewport's rendering. Must be explicitly written to in renderer script.
> ``` lang=cpp, name=Lightning
> var FinalTexture : Texture


---  
 #  ForwardViewportEvents : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Forwards mouse events to viewports underneath this viewport.
> ``` lang=cpp, name=Lightning
> var ForwardViewportEvents : Boolean


---  
 #  Frustum : [frustum](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/frustum.markdown)

 `read-only`

> Creates a frustum using the CameraViewport's settings (including aspect ratio). If the Camera is null, then this will throw an exception.
> ``` lang=cpp, name=Lightning
> var Frustum : Frustum


---  
 #  MarginColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4.markdown)

> Color to used for letterbox/scaling margins.
> ``` lang=cpp, name=Lightning
> var MarginColor : Real4


---  
 #  MouseWorldRay : [ray](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown)

 `read-only`

> Get the world ray starting from the mouse.
> ``` lang=cpp, name=Lightning
> var MouseWorldRay : Ray


---  
 #  NormalizedOffset : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Offset of the viewport in normalized UI coordinates.
> ``` lang=cpp, name=Lightning
> var NormalizedOffset : Real2


---  
 #  NormalizedSize : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Size of viewport in normalized UI coordinates.
> ``` lang=cpp, name=Lightning
> var NormalizedSize : Real2


---  
 #  RendererPath : [cogpath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cogpath.markdown)

> Object with renderer script that connects to RenderTasksUpdate that determines what rendering will be done.
> ``` lang=cpp, name=Lightning
> var RendererPath : CogPath


---  
 #  RenderInEditor : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If rendering will be ran in edit mode.
> ``` lang=cpp, name=Lightning
> var RenderInEditor : Boolean


---  
 #  RenderInGame : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If rendering will be ran in play game mode.
> ``` lang=cpp, name=Lightning
> var RenderInGame : Boolean


---  
 #  RenderOrder : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

> The order that rendering should be done relative to other CameraViewports, lowest to highest.
> ``` lang=cpp, name=Lightning
> var RenderOrder : Integer


---  
 #  RenderToViewport : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> If the rendering result in FinalTexture should also be placed on the UI viewport.
> ``` lang=cpp, name=Lightning
> var RenderToViewport : Boolean


---  
 #  ResolutionOrAspect : [integer2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer2.markdown)

> 
> ``` lang=cpp, name=Lightning
> var ResolutionOrAspect : Integer2


---  
 #  ViewportHasFocus : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> If the viewport created by this CameraViewport, if rendering to one, has focus.
> ``` lang=cpp, name=Lightning
> var ViewportHasFocus : Boolean


---  
 #  ViewportOffset : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

 `read-only`

> The current offset of the viewport, in pixels.
> ``` lang=cpp, name=Lightning
> var ViewportOffset : Real2


---  
 #  ViewportOffsetWithMargin : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

 `read-only`

> The current offset of the viewport's margin, in pixels.
> ``` lang=cpp, name=Lightning
> var ViewportOffsetWithMargin : Real2


---  
 #  ViewportResolution : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

 `read-only`

> The current resolution of the viewport.
> ``` lang=cpp, name=Lightning
> var ViewportResolution : Real2


---  
 #  ViewportResolutionWithMargin : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

 `read-only`

> The current resolution of the viewport including margin.
> ``` lang=cpp, name=Lightning
> var ViewportResolutionWithMargin : Real2


---  
 #  ViewportScaling : [ViewportScaling](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#viewportscaling)

> Method to use for sizing the viewport.
> ``` lang=cpp, name=Lightning
> var ViewportScaling : ViewportScaling


---  
 #  ViewToPerspective : [real4x4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4x4.markdown)

 `read-only`

> Transformation that defines how the view frustum is mapped to normalized coordinates, pre W divide.
> ``` lang=cpp, name=Lightning
> var ViewToPerspective : Real4x4


---  
 #  WorldToPerspective : [real4x4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4x4.markdown)

 `read-only`

> Concatenation of the WorldToView and ViewToPerspective transformations.
> ``` lang=cpp, name=Lightning
> var WorldToPerspective : Real4x4


---  
 #  WorldToView : [real4x4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4x4.markdown)

 `read-only`

> Transformation that defines view space as the Camera at the origin and the view direction as -Z.
> ``` lang=cpp, name=Lightning
> var WorldToView : Real4x4


---  
 #  Methods


---  
 #  CameraViewport : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CameraViewport()
> ``` 


---  
 #  ScreenToViewport : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Convert a screen point to a point relative to the viewport.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function ScreenToViewport(screenPoint : Real2) : Real2
> ``` 


---  
 #  ScreenToWorldPlane : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Convert the screen point to a position on a given plane.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> |worldPlaneNormal|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |worldPlanePosition|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function ScreenToWorldPlane(screenPoint : Real2, worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ScreenToWorldRay : [ray](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/ray.markdown)

> Convert a screen point to a ray.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function ScreenToWorldRay(screenPoint : Real2) : Ray
> ``` 


---  
 #  ScreenToWorldViewPlane : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Convert the screen point to a position on the view plane at a given depth.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> |viewDepth|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function ScreenToWorldViewPlane(screenPoint : Real2, viewDepth : Real) : Real3
> ``` 


---  
 #  ScreenToWorldZPlane : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Convert the screen point to a position on the z plane at a given depth.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> |worldDepth|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function ScreenToWorldZPlane(screenPoint : Real2, worldDepth : Real) : Real3
> ``` 


---  
 #  ViewPlaneSize : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Size of the screen at a Depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function ViewPlaneSize(viewDepth : Real) : Real2
> ``` 


---  
 #  ViewportTakeFocus : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Returns whether or not it succeeded in taking focus. Will always fail if RenderToViewport is false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ViewportTakeFocus() : Boolean
> ``` 


---  
 #  ViewportToScreen : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Convert a viewport point to a screen point.
> |Name|Type|Description|
> |---|---|---|
> |viewportPoint|[real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)| |
> ``` lang=cpp, name=Lightning
> function ViewportToScreen(viewportPoint : Real2) : Real2
> ``` 


---  
 #  WorldToScreen : [real2](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real2.markdown)

> Convert a world point to a screen point.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function WorldToScreen(worldPoint : Real3) : Real2
> ``` 


---  
 

 
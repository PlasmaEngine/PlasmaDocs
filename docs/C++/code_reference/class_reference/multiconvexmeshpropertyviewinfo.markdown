 `Editor`

(NOTE) Structure bound to the property view for the main editor. Contains the different settings that the user can modify.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AutoCompute](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#autocompute-void)|[ AutoComputeMethod](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#autocomputemethod-plasma-e)|[eventobject](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/eventobject.markdown)| |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#multiconvexmeshpropertyv)|[ AutoComputeMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#autocomputemode-plasma-eng)| | |
| |[ ClearColor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#clearcolor-plasma-engine-d)| | |
| |[ DrawMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#drawmode-plasma-engine-doc)| | |
| |[ MeshThickness](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#meshthickness-plasma-engin)| | |
| |[ OuterContourColor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#outercontourcolor-plasma-e)| | |
| |[ SimplificationThreshold](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#simplificationthreshold)| | |
| |[ SpriteSource](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#spritesource-plasma-engine)| | |
| |[ SurfaceLevelThreshold](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/multiconvexmeshpropertyviewinfo.markdown#surfacelevelthreshold-ze)| | |


 #  Properties


---  
 #  AutoComputeMethod : [MultiConvexMeshAutoComputeMethod](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#multiconvexmeshautocomputemethod)

> What method of auto-computing should be used? Most likely 'pixel' is the mode that should be used.
> ``` lang=cpp, name=Lightning
> var AutoComputeMethod : MultiConvexMeshAutoComputeMethod


---  
 #  AutoComputeMode : [MultiConvexMeshAutoComputeMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#multiconvexmeshautocomputemode)

> Should the auto-computed mesh be calculated from the alpha or the intensity of the sprite?
> ``` lang=cpp, name=Lightning
> var AutoComputeMode : MultiConvexMeshAutoComputeMode


---  
 #  ClearColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> The clear color of the viewport used to render.
> ``` lang=cpp, name=Lightning
> var ClearColor : Real4


---  
 #  DrawMode : [MultiConvexMeshDrawMode](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#multiconvexmeshdrawmode)

> How should the collection of meshes be drawn?
> ``` lang=cpp, name=Lightning
> var DrawMode : MultiConvexMeshDrawMode


---  
 #  MeshThickness : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> Since the mesh is on a 2d plane, they need some thickness for their z-depth. This controls how thick the meshes are.
> ``` lang=cpp, name=Lightning
> var MeshThickness : Real


---  
 #  OuterContourColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> The color to draw edges with.
> ``` lang=cpp, name=Lightning
> var OuterContourColor : Real4


---  
 #  SimplificationThreshold : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> A threshold to control when vertices should be removed (simplified). This value is related to the area of a triangle.
> ``` lang=cpp, name=Lightning
> var SimplificationThreshold : Real


---  
 #  SpriteSource : [spritesource](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritesource.markdown)

> The sprite source used as a reference for drawing the mesh. Note: this is not always what's visible as the user can drag in archetypes to view as well.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  SurfaceLevelThreshold : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> When the sprite is sampled using the AutoComputeMode, what value should be used to determine where a surface is.
> ``` lang=cpp, name=Lightning
> var SurfaceLevelThreshold : Real


---  
 #  Methods


---  
 #  AutoCompute : Void

> Resets the points of the mesh to an approximation for the current sprite.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function AutoCompute()
> ``` 


---  
 #  MultiConvexMeshPropertyViewInfo : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MultiConvexMeshPropertyViewInfo()
> ``` 


---  
 

 
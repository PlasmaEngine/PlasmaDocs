 `Editor`

(NOTE) Structure bound to the property view for the main editor. Contains the different settings that the user can modify.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AutoCompute](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocompute-void)|[ AutoComputeMethod](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocomputemethod-plasma-e)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.md)| |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#multiconvexmeshpropertyv)|[ AutoComputeMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocomputemode-plasma-eng)| | |
| |[ ClearColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#clearcolor-plasma-engine-d)| | |
| |[ DrawMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#drawmode-plasma-engine-doc)| | |
| |[ MeshThickness](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#meshthickness-plasma-engin)| | |
| |[ OuterContourColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#outercontourcolor-plasma-e)| | |
| |[ SimplificationThreshold](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#simplificationthreshold)| | |
| |[ SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#spritesource-plasma-engine)| | |
| |[ SurfaceLevelThreshold](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#surfacelevelthreshold-ze)| | |


 #  Properties


---  
 #  AutoComputeMethod : [MultiConvexMeshAutoComputeMethod](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#multiconvexmeshautocomputemethod)

> What method of auto-computing should be used? Most likely 'pixel' is the mode that should be used.
> ``` lang=cpp, name=Lightning
> var AutoComputeMethod : MultiConvexMeshAutoComputeMethod


---  
 #  AutoComputeMode : [MultiConvexMeshAutoComputeMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#multiconvexmeshautocomputemode)

> Should the auto-computed mesh be calculated from the alpha or the intensity of the sprite?
> ``` lang=cpp, name=Lightning
> var AutoComputeMode : MultiConvexMeshAutoComputeMode


---  
 #  ClearColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> The clear color of the viewport used to render.
> ``` lang=cpp, name=Lightning
> var ClearColor : Real4


---  
 #  DrawMode : [MultiConvexMeshDrawMode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#multiconvexmeshdrawmode)

> How should the collection of meshes be drawn?
> ``` lang=cpp, name=Lightning
> var DrawMode : MultiConvexMeshDrawMode


---  
 #  MeshThickness : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Since the mesh is on a 2d plane, they need some thickness for their z-depth. This controls how thick the meshes are.
> ``` lang=cpp, name=Lightning
> var MeshThickness : Real


---  
 #  OuterContourColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> The color to draw edges with.
> ``` lang=cpp, name=Lightning
> var OuterContourColor : Real4


---  
 #  SimplificationThreshold : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> A threshold to control when vertices should be removed (simplified). This value is related to the area of a triangle.
> ``` lang=cpp, name=Lightning
> var SimplificationThreshold : Real


---  
 #  SpriteSource : [spritesource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritesource.md)

> The sprite source used as a reference for drawing the mesh. Note: this is not always what's visible as the user can drag in archetypes to view as well.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  SurfaceLevelThreshold : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

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
 

 
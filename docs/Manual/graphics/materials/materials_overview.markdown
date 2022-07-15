# Materials
[Materials](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/material.markdown), and the parameters found in them, define the shader for drawing objects for any purpose, using any renderer. Their overarching, generalized purpose is to house shader code (pixel, vertex, and geometry) using individual LightningFragments. These LightningFragments added to a Material as MaterialBlocks. These [ shader fragments ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/shaders.markdown) define how the surface of the object on which it is placed will react to its environment.  [PBR](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/physically_based_rendering.markdown), which is provided for the user as the default [DeferredRenderer](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/renderer/deferred_renderer.markdown#deferred-renderer), is just one instance of how Materials may be used to render objects. To add a new Material, see [Adding a Resource](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorcommands/resourceadding.markdown).

# Material Templates

When creating a new material, there are six templates from which to choose:

|Template | Description|
|--|--|
|`PlasmaMaterial`| PBR-based material defined by TextureMaps|
|`OpaqueFlat`| PBR-based material defined by uniform values |
|`EmptyMaterial`| Free of any default MaterialBlocks or references to [RenderGroups](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/rendergroups.markdown) |
|`AdditiveSprite`| Used for sprites that require additive blending |
|`AlphaCut`| Used for graphicals that should be alpha cut |
|`AlphaSprite`| Used for sprites that require alpha blending |

Each of these templates has MaterialBlocks and references to RenderGroups pre-added. The PlasmaMaterial, for example, has `AlbedoMap`, `NormalMap`, `RoughnessMap`, `MetallicMap`, and `SpecularValue` MaterialBlocks and references `Opaque`, and `ShadowCasters` RenderGroups.

[ Albedo ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/albedo.markdown), [ Normal ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/normal_map.markdown), [ Metallic ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/metallic.markdown), [ Roughness ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/roughness.markdown), and Specular are the parameters that define how light interacts with the material. Each of these parameters may be defined by a texture map or by a value, with the exception of the Normal parameter which may only be defined by a map.

# Related Materials
## Manual
- [rendergroups](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/rendergroups.markdown)
- [model_component](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/models/model_component.markdown)
- [materials](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials.markdown)
- [ Albedo ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/albedo.markdown)
- [ Normal ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/normal_map.markdown)
- [ Metallic ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/metallic.markdown)
- [ Roughness ](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/roughness.markdown)
- [shaders](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/materials/shaders.markdown)

## Code Reference
- [rendergroup](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/rendergroup.markdown) 
- [model](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/model.markdown)
- [material](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/material.markdown) 

 
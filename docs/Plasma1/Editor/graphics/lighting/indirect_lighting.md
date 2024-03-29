# Indirect lighting
Indirect lighting in Plasma takes the form of image-based lighting, where an image--primarily a skybox--provides environmental ambient lighting throughout a scene. Whether a skybox is artist-created or derived from HDR images, is often used to give a scene an ambient light associated with a certain time of day (e.g. dusk, noon, dawn) or certain types of weather (e.g. clear skies, threatening clouds). In the case of interior scenes, it may just provide a static ambient light so that no matter where in the scene a player is, objects maintain some level of visibility.

When using a skybox, it may be either visible, providing a static background for a scene (e.g. clouds in a sky) or invisible, in which the skybox provides ambient light for an interior scene (e.g. a cave that needs to have a constant source of ambient light not provided by [deferred or forward renderer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/renderer/deferred_renderer.md).

NOTE: If a skybox is used and is visible, [MipMapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#texturemipmapping) on the skybox [TextureBuilder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/adding_assets/adding_textures_and_sprites.md) ContentComponent must be set to `PreGenerated`.

When applying indirect lighting to scene, the math used is the same as is used when applying [direct lighting](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/lighting/direct_lighting.md). The only difference between the two is that much of the math is pre-calculated for indirect lighting. 

 
# Importing Sprites
[SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritesource.markdown) is the Resource used to create [Sprites](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/sprite.markdown), which represent all 2D graphical assets in Plasma.  Sprites can take the form of a single 2D image or a SpriteSheet displaying all the Sprites needed for an animation in the same file. See [resourceadding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/editorcommands/resourceadding.markdown) for how to import an image as a SpriteSource.

NOTE: The only file format that may be imported to create a SpriteSource is `.png`. Other formats, such as `.jpg`, are lossy and can result in undesirable artifacts, especially when scaled. If the image only exists as a `.jpg` and it is absolutely necessary, there are a number of websites that offer free conversion from `.jpg` (and many other formats) to `.png`.

# SpriteSource Setup
To change the values applied to a SpriteSource when an image is imported, double-click the appropriate SpriteSource from the Library window window, which will open the [Sprite Source Editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/spritesourceeditor.markdown):

![SpriteSourceEditor](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/SpriteImportFull.PNG) 

There are many different properties that may be modified such as where to set the origin, the type of sampling, and the SpriteFill mode (to change from Fill to [Nine Slice](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/area.markdown) for example). If the SpriteSource is a sprite sheet created for [ Sprite animation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/spritesourceeditor.markdown#creating-sprite-animatio), click on `Convert to Animation` to open the Sprite Importer window.

# Related Material

## Manual
 [BaseSprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/basesprite.markdown)
 [Sprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/sprite.markdown)
 [Sprite Source Editor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/sprites/spritesourceeditor.markdown)
 [Block Compression](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/adding_assets/block_compression.markdown)

## Reference
 [SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/spritesource.markdown) 
 [Sprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/sprite.markdown)  

 
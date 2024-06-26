# ImageData Asset

The *image data asset* references an image file (png, jpg, etc). However, contrary to a [texture](textures-overview.md), an *image data* resource is **not used for rendering**, but instead is available to be sampled on the CPU. That means, it simply represents two-dimensional data with 4 floating point channels.

For example the [heightfield component](heightfield-component.md) uses an image data asset to determine the height of each vertex by reading it from an image file.

## See Also


* [Textures](textures-overview.md)
* [Heightfield Component](heightfield-component.md)

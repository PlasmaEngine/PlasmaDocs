# Shaders
Shaders may be added to Plasma in the form of LightningFragments, allowing the user to write shaders using the Lightning language. Zero currently supports the following types of shaders:

 - **Pixel** - Operates on individual pixels, setting and changing their properties.
 - **Vertex** - Operates on individual vertices, setting and changing their properties.
 - **Geometry** - Operates on transformed primitives (e.g. point, lines,  triangles), setting and changing their properties.
 - **PostProcess** - Operates on the window of an entire scene, after that scene has been processed.

When adding a new LightningFragment, there are multiple templates for each type of shader:

| Shader | Template |  Description |
| ---|---|--- |
| Pixel | Pixel Annotated |  All of the built-in inputs  that may be used have been commented. |
| Pixel | Pixel Empty |   No inputs or outputs pre-defined. |
| Pixel | Pixel Normal Map |  Uses a NormalMap to perturb the surface normal |
| Vertex | Vertex Annotated |  All of the built-in inputs that may be used have been commented. |
| Vertex | Vertex Empty |  No inputs or outputs pre-defined. |
| Vertex | Vertex Oscillate |  Demonstration of a vertex shader that applies a simple oscillation to all vertices. |
| Geometry | Point To Quad |  Demonstration of generating geometry, creating quads from points. |
| Geometry | Polygon Normals | Demonstration of manipulating geometry, changing normals of a triangle. |
| PostProcess | Post Process Blur | Applies a simple post-process blur effect. |
| PostProcess | Post Process Copy | Copies a texture. |


# Shader Translation Debug Helper

This tool translates Materials (rather, the LightningFragments that make up the Material) into different versions of the shader language GLSL.

[Command](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/editorcommands/commands.md) : [ DebugShaderTranslation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/command_reference.md#debugshadertranslation) will open the tool

On the left hand side of the window are properties that set the parameters that define the shaders to be be translated: CoreVertex enum, Material enum, and RenderPass enum. `Translation Language` set the version of GLSL to translate to.  These options set what exactly will be translated. Material enum, for example, sets the Material to be translated as its name would suggest.

If not familiar with GLSL, these will become overwhelmingly complex very quickly. With at least an intermediate amount of experience in GLSL, however, this translator provides a valuable tool for debugging your LightningFragment shaders. Changing the other attributes to different settings will result in different outputs, so try to make sure that the attributes selected line up to the location on the render pipeline.

# Related Materials
## Manual
- [normal_map](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/materials/normal_map.md)
- [Material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/materials/materials_overview.md)
 

 
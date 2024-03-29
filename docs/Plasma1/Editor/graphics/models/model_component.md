# Model Component
The Model component allows the user to assign a [Mesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mesh.md) and a [ Material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/graphics/materials/materials_overview.md) to an object.

# Material and Mesh

These properties are where the Material and Mesh resources for the model are set. If a model has been imported using a scene asset file,  the archetype for the object will have the Mesh associated with a specific object already set. By default, the Material will be set to the PlasmaMaterial until changed by the user.  If using the SkinnedModel component, the Mesh resource should be a skinned mesh. 

# Skinned Model

The only property the SkinnedModel component has that the Model component does not is SkeletonPath. When a skinned mesh is imported, SkeletonPath is automatically set to whatever object the animation takes as its first target (i.e. the root object of a skeleton of the generated hierarchy).  The object that SkeletonPath points to should have the Skeleton component on it as well as being the root object of the entire skeleton (i.e. the parent object of all of the bone objects). If SkeletonPath is set incorrectly, the object will fail to animate as the SkinnedModel receives all of its transformation data from the skeleton.

# Related Materials
## Reference
- [Model](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/model.md)
- [SkinnedModel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/skinnedmodel.md)
- [Mesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/mesh.md)
- [Material](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/code_reference/class_reference/material.md)
 

 
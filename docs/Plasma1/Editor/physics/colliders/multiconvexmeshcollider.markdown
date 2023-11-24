# Multi Convex Mesh Collider
(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.markdown) page should be read before this page.

[MultiConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshcollider.markdown) defines a collection of [convex hulls](https://en.wikipedia.org/wiki/Convex_hull ) for collision detection based upon a [MultiConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.markdown) resource.

WARNING: A future version will likely combine all physics mesh types together.

MultiConvexMeshCollider allows more complicated shapes to be represented than a [ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/convexmeshcollider.markdown) while still retaining performance. Physics needs convex shapes for efficiency so this Collider represents non-convex shapes as a collection of sub convex meshes.

Currently, the editor for this mesh type only works for 2D shapes (sprites). 3D meshes can be made, but only through script. Future plans include implementing 3D approximate convex decomposition.

# Troubleshooting
As the MultiConvexMeshCollider contains multiple convex pieces, seams can exist between the pieces. This can cause [edge catching](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/physicstroubleshooting/edgecatching.markdown) issues when objects slide across the surface. Additionally, an object can get sandwiched in the interior between two sub-meshes.

# Related Materials
## Manual
- [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.markdown)
- [convexmeshcollider.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/convexmeshcollider.markdown)
- [edgecatching.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/physicstroubleshooting/edgecatching.markdown)

## Reference
- [MultiConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshcollider.markdown)
- [MultiConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.markdown)
- [ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmeshcollider.markdown)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown) 

 
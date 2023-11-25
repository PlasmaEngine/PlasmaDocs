# Multi Convex Mesh Collider
(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md) page should be read before this page.

[MultiConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshcollider.md) defines a collection of [convex hulls](https://en.wikipedia.org/wiki/Convex_hull ) for collision detection based upon a [MultiConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md) resource.

WARNING: A future version will likely combine all physics mesh types together.

MultiConvexMeshCollider allows more complicated shapes to be represented than a [ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/convexmeshcollider.md) while still retaining performance. Physics needs convex shapes for efficiency so this Collider represents non-convex shapes as a collection of sub convex meshes.

Currently, the editor for this mesh type only works for 2D shapes (sprites). 3D meshes can be made, but only through script. Future plans include implementing 3D approximate convex decomposition.

# Troubleshooting
As the MultiConvexMeshCollider contains multiple convex pieces, seams can exist between the pieces. This can cause [edge catching](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/physicstroubleshooting/edgecatching.md) issues when objects slide across the surface. Additionally, an object can get sandwiched in the interior between two sub-meshes.

# Related Materials
## Manual
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md)
- [convexmeshcollider.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/convexmeshcollider.md)
- [edgecatching.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/physicstroubleshooting/edgecatching.md)

## Reference
- [MultiConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmeshcollider.md)
- [MultiConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/multiconvexmesh.md)
- [ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmeshcollider.md)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md) 

 
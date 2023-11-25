# Convex Mesh Collider
(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md) page should be read before this page.

[ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmeshcollider.md) defines a [convex hull](https://en.wikipedia.org/wiki/Convex_hull ) for collision detection based upon a [ConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.md) resource.

WARNING: A future version will likely combine all physics mesh types together.

Unlike [MeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/meshcollider.md), convex meshes have a volume which means inertia properties can be computed. ConvexMeshColliders are complex shapes that are still efficient for physics. They are commonly used with dynamic rigid bodies to create an object with a complicated surface.

If a mesh is non-convex, the convex hull of the shape is used for collision detection. This means that the geometry will be an approximation of the surface. 

# Related Materials
## Manual
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md)
- [meshcollider.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/meshcollider.md)

## Reference
- [ConvexMeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmeshcollider.md)
- [ConvexMesh](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/convexmesh.md)
- [MeshCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/meshcollider.md)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md) 

 
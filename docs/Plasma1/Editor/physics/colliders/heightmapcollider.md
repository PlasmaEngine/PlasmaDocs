# Height Map Collider
(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md) page should be read before this page.

[HeightMapCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md) defines collision for a [HeightMap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmap.md). Physics more efficiently represent collision for a HeightMap than a generic mesh.

NOTE: HeightMapCollider is assumed to be static and should not be used with a dynamic [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/rigidbody.md).

## Thickness
HeightMapCollider exposes the Thickness  property to turn each triangle of the height map into a [prism](https://en.wikipedia.org/wiki/Triangular_prism ). This helps avoid tunneling with fast moving objects.

# Related Materials
## Manual
 - [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md)
 - [rigidbody.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders/rigidbody.md)

## Reference
 - [HeightMapCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmapcollider.md)
 - [HeightMap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/heightmap.md)
 - [RigidBody](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rigidbody.md) 

 
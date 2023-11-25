# Box Collider
[BoxCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.md) defines a rectangular box shape ([cuboid](https://en.wikipedia.org/wiki/Cuboid )) for collision. The size of the box is determined by the combination of the box's Size  property and the Transform's Scale .

(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md) page should be read before this page.

## Size
A BoxCollider exposes the Size  property to determine the pre-transform size of this box. This is most commonly done to match the collision to graphics before scale is applied. Additionally, this is sometimes used to set the size of a root object's collision without running into non-uniform scale issues.

# Related Materials
## Manual
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md)

## Reference
- [BoxCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.md)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md) 

 
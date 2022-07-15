# Box Collider
[BoxCollider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/boxcollider.markdown) defines a rectangular box shape ([cuboid](https://en.wikipedia.org/wiki/Cuboid )) for collision. The size of the box is determined by the combination of the box's Size  property and the Transform's Scale .

(NOTE) **Recommended Reading:** The [Collider](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/colliders.markdown) page should be read before this page.

## Size
A BoxCollider exposes the Size  property to determine the pre-transform size of this box. This is most commonly done to match the collision to graphics before scale is applied. Additionally, this is sometimes used to set the size of a root object's collision without running into non-uniform scale issues.

# Related Materials
## Manual
- [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/colliders.markdown)

## Reference
- [BoxCollider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/boxcollider.markdown)
- [Collider](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/collider.markdown) 

 
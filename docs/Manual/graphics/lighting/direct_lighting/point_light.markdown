# point light
A point light is a light that has a defined shape, exists at particular point in space, and sends light out equally from all points on that shape. It uses a sphere [mesh](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/mesh.markdown) to define its volume, as can be seen on the [Model component](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/models/model_component.markdown). The light that is emitted will only be processed on geometry that the light overlaps, which is found using a special depth test unique to the point light.

# LightIntensity and LightRadius

LightIntensity  falls off as the distance increases from the surface of the light as defined by the LightRadius . The fall off follows the inverse square law. The LightIntensity  and FalloffRadius  are independent from each other. 

LightRadius  defines the size of the "physical" object that represents the object emitting the light. This "physical" object that can only be seen in the reflection of the PointLight (see screenshots below) As this radius approaches plasma, it comes to represent an infinitely small point. As the radius increases and the intensity stays the same, the light emitted will be spread out as the same intensity must now be spread across the surface of a larger object. When the value LightRadius  increases, the size of the specular, or reflected, light grows. This is most obvious when looking at the reflection of the light source: the sphere reflected on the surface of the floor and wall objects gets larger. As the specular light increases, however, the intensity also dims, as the amount of energy emitted remains the same despite increasing the area from which it is emitted.

# FalloffRadius

FalloffRadius  defines the size of the sphere mesh that acts as the volume in which emitted light may be processed. If the value defines a volume larger than what the emitted light would reach, increasing it any further will have no effect. If the value defines a volume below what the emitted light would reach, the intensity falloff is truncated.

# Related Materials

## Manual
- [Model component](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/models/model_component.markdown)

## Code Reference
- [Mesh](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/mesh.markdown) 

 
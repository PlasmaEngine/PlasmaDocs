# Flow Effect
The [FlowEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown) component applies forces to make an object move at a target speed in a given direction. This is often used to make an object move in the flow of another, such as a river or a tractor beam.

![FlowEffect](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46701.png)


Unlike a [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/forceeffect.markdown) which applies a constant force in a direction, FlowEffect applies a variable force to make an object move at a constant speed in the flow direction. MaxFlowForce  allows the user to control how much force can be applied to reach this target speed. This can also be thought of as controlling the acceleration of objects within the field. Note: the flow portion of the effect only affects movement in the flow direction, not in the inward force direction.

Additionally, FlowEffect has the AttractToFlowCenter checkBox property to pull objects towards the flow center. This attractional force is similarly defined by a target speed and a max force. Note: this force only affects movement in the inward direction, not in the flow direction.

 #  Application Modes
FlowEffect is only expected to be used as a [Region](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/region.markdown) effect. Other application modes are undefined.

---
 #  Related Materials
 ##  Manual
- [physicseffectsandregions.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions.markdown)
- [forceeffect.markdown](https://plasmaengine.github.io/PlasmaDocs/Manual/physics/physicseffectsandregions/forceeffect.markdown)

 ##  Reference
- [FlowEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/floweffect.markdown)
- [ForceEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/forceeffect.markdown)
- [PhysicsEffect](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/physicseffect.markdown)
- [Region](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/region.markdown)
 

 
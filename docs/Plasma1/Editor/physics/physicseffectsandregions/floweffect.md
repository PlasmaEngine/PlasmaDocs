# Flow Effect
The [FlowEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md) component applies forces to make an object move at a target speed in a given direction. This is often used to make an object move in the flow of another, such as a river or a tractor beam.

![FlowEffect](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46701.png)


Unlike a [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/forceeffect.md) which applies a constant force in a direction, FlowEffect applies a variable force to make an object move at a constant speed in the flow direction. MaxFlowForce  allows the user to control how much force can be applied to reach this target speed. This can also be thought of as controlling the acceleration of objects within the field. Note: the flow portion of the effect only affects movement in the flow direction, not in the inward force direction.

Additionally, FlowEffect has the AttractToFlowCenter checkBox property to pull objects towards the flow center. This attractional force is similarly defined by a target speed and a max force. Note: this force only affects movement in the inward direction, not in the flow direction.

 #  Application Modes
FlowEffect is only expected to be used as a [Region](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.md) effect. Other application modes are undefined.

---
 #  Related Materials
 ##  Manual
- [physicseffectsandregions.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions.md)
- [forceeffect.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicseffectsandregions/forceeffect.md)

 ##  Reference
- [FlowEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/floweffect.md)
- [ForceEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/forceeffect.md)
- [PhysicsEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.md)
- [Region](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.md)
 

 
# Joints

[Joints](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md) are a representation of a physics concept known as [constraints](https://en.wikipedia.org/wiki/Constraint_(mathematics) ). A constraint is a mathematical rule that defines (or constrains) how objects are allowed to move. A Joint is a collection of one or more constraints that define a more common interaction. In Plasma, a Joint is typically an independent object that connects two [ObjectLink](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/objectlink.md).

# Shared Properties

Before looking at individual joints, there's a few useful shared properties:
 - Active checkBox Any joint can be toggled in order to temporarily disable it.
 - CollideConnected checkBox Sometimes it's useful to disable collision between the two objects the joint is connected to (e.g. articulated bodies).
 - MaxImpulse  The max impulse (instantaneous force) allowed for the joint to solve any of its constraints. 'JointExceedImpulseLimit' is sent when this happens.
 - AutoSnaps checkBox It's common to auto-delete a joint when the MaxImpulse  is exceeded. This property provides this behavior without requiring scripting.

# Joint Add-ons

Before discussing each individual Joint, there's several helper components that are important to understand. These components affect how a joint will affect the connected objects. These components can be added to any Joint, but may not always make sense for a specific one.

### [JointLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md)

A limit restricts a certain portion of the joint to only be active part of the time. This is typically sets some min/max distance/angle where the joint will allow free movement.
NOTE: When the limit is for angles it is specified in radians.

### [JointMotor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md)

A motor takes a portion of the joint and adds energy to it. This is often used to drive a portion of the joint when no external forces are acting upon it. A motor allows setting a target speed and a max impulse it can use to try and achieve this.

### [JointSpring](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointspring.md)

A spring takes a portion of the joint and makes it soft, or non-rigid. This can be useful to simulate a spring or make the limits of a joint springy. Springs are defined by a frequency in Hertz (oscillations per second) and a damping ratio. The damping ratio defines how much energy should be damped out of the system where 0 means no damping and 1 is critical (perfect) damping.

## Extra AddOns

There are a few extra joint add-ons that are less frequently used.

### [JointConfigOverride](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md)

This allows configuring individual joint properties for solving. Typically you shouldn't touch this if you don't understand it.

### [JointDebugDrawConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md)

The debug draw config is used to give additional debug drawing information to the joint. This is mostly to allow configuring which object's perspective to draw information from. Not all joints currently observe this component.

# JointTypes

The physics systems supports most common mechanical joint types.

### StickJoint

A stick joint, or distance joint, defines that two points on the objects should be a certain distance apart. This is common for creating rope-like objects.

### PositionJoint

A position joint locks two points on the objects to be at the same position. This is common for a ball-and-socket like joint.

### WeldJoint

A weld joint locks the the relative position and rotation of two objects together. For a rigid connection, [hierarchies](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/hierarchies.md) should be used instead as joints are not completely stiff. If run-time behaviors, such as auto-snapping with a max impulse, are desired then using a weld is easier than hierarchies.

### PrismaticJoint

A prismatic joint (or slider) locks the rotation of two objects together and two of the linear axes. This allows relative translation of the objects along one axis. This is often used to create pistons or sliders.

### RevoluteJoint

A revolute joint (or hinge) locks the positions of two objects together and two of the rotational axes. This allows relative rotation of the objects along one axis. This is often used to create doors, wheels, seesaws, etc....

### WheelJoint

A wheel joint is a revolute joint with a spring on one of the translational axes. This allows the axis to act like a suspension.

### UniversalJoint

A universal joint locks the positions of two objects together and one of the rotational axes. This allows relative rotation about two axes. This joint is currently in a prototype state.

### UprightJoint

The upright joint locks the rotation about one axis of two objects together. This is often used to keep an object always pointing up (or close enough).

### GearJoint

The gear joint connects two joints of two objects together. The expected joint types to connect are prismatic or revolute. This makes the two joints transfer energy between each other to make more complicated joints.

### PulleyJoint

A pulley joint connects two stick joints on two objects together. This restricts the relative length of the two joints together to create a pulley system.

### CustomJoint

A custom joint is for advanced users. This allows you to define your own constraints via Jacobians and other constraint definitions.

## 2D Joints

A few joints have 2D versions that should be used when making a 2D game instead of their 3D counterpart. The 2D versions makes certain assumptions about axes that don't need to be solved which result in faster performance and increased stability.

## Related Materials
### Manual
- [colliders.md](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/colliders.md)

### Reference
 - [Joint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joint.md)
 - [StickJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/stickjoint.md)
 - [PositionJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjoint.md)
 - [WeldJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/weldjoint.md)
 - [PrismaticJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint.md)
 - [PrismaticJoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2d.md)
 - [RevoluteJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint.md)
 - [RevoluteJoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint2d.md)
 - [WheelJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint.md)
 - [WheelJoint2d](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint2d.md)
 - [UniversalJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljoint.md)
 - [UprightJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjoint.md)
 - [GearJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjoint.md)
 - [PulleyJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjoint.md)
 - [CustomJoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjoint.md)
 - [JointEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointevent.md)
 - [CustomJointEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointevent.md)
 - [JointLimit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointlimit.md)
 - [JointMotor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointmotor.md)
 - [JointSpring](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointspring.md)
 - [JointDebugDrawConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointdebugdrawconfig.md)
 - [JointConfigOverride](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/jointconfigoverride.md)
 - [CustomConstraintInfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customconstraintinfo.md)
 - [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.md)
 

 
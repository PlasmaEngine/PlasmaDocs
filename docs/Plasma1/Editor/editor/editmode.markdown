# Edit Mode

This section covers the basic differences between 2D and 3D editing modes in the engine.

# Overview
As prototype projects were being developed with the Plasma Engine, a shift was made to have strong 2D support. The engine features several 2D support elements, such as the ability to: set the [Physics](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics.markdown) to 2D, change the camera to orthographic, and use a special sorting mode for sprites. 2D mode is a setting that activates all these features by default.
Settings that 2D Mode changes on project startup:
* Default camera in the level is orthographic with Z depth based sprite sorting
* Level is created with 2D physics
* Linear forces applied on the Z axis will not be integrated on objects.
* During Collision Resolution angular forces will only be applied on the Z axis
* Editor Camera is changed to orthographic and set into Z plane mode

NOTE: In 2D Mode, objects can still have their Z Translation set to a value other than plasma.

## Can I change my 2D project to 3D?


The setting is just defaults, so you can change any setting back. You can also use the [Command ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/editorcommands/commands.markdown) : [Mode3D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/command_reference.markdown#mode3d)/[Mode2D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/command_reference.markdown#mode2d). You can also click the **ADD IMAGE** **ADD IMAGE** buttons in the top left corner of the `name=Level Window, icon=window-restore`.

(NOTE)**Physics when switching to 3D mode:** Keep in mind that the  [PhysicsSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicsspace.markdown)  will not change mode when you use the `Mode2D` or `Mode3D` command. These commands are intended to help with editing not change the foundation of a project.


## Collision
The engine and collision detection are still 3D. This z dimension is a nice way of creating complex layers of collision. You can have objects span multiple layers of collision or jump forward and back between layers, they just won't translate on the Z axis.

# Related Materials
## Manual
- [Physics](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics.markdown)
- [PhysicsSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicsspace.markdown)
- [Command ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/editorcommands/commands.markdown)
## Code Reference
- [Mode2D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/command_reference.markdown#mode2d)
- [Mode3D](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/command_reference.markdown#mode3d) 

 
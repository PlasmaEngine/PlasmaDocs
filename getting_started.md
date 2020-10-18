 #  [Download the Engine](https://plasmagameengine.com/ )
 - [min_specs.markdown](https://github.com/PlasmaEngine/PlasmaDocs/blob/master//Users/beepboopowner/Desktop/AJ/DP/getting_started/min_specs.markdown)

 # Installing the Plasma Engine (and Plasma Launcher)

The Plasma Engine is downloaded through the Plasma Launcher, this allows to the installation and manamagement of multiple engine versions along with the
creation and management of projects. This is all designed to make the life of the user as easy as possible.

 - [Learn how to use the Plasma Launcher](https://github.comPlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor/launcher.markdown).

 # Plasma Engine Features
The Plasma Engine is capable of creating a wide veriaty of project from 2D Platformers to 3D First Person Shooters and beyond. Everything within Plasma is designed to be as extendable as possible for the users. So if your focus is on Graphics, Physics, Gameplay or anything else you can make Plasma your engine of choice.
The versatility of the engine is made possible by the features in the following sections:

 ## [Ecosystem](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor.markdown)
 - A discrete [launcher](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor/launcher.markdown) that provides access to all project and engine builds
 - A wider selection of templates and sample project to help build your dreams
 - Direct communication with the development team via discord
  
 ## [Editor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor.markdown)
 - [Editor modes](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor/editmode.markdown) customized for both 2D and 3D projects
 - Full-featured [text editor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor/texteditor.markdown) and programming enviroment with many configurable options
 - Script debugging and breakpoints in editor
 - Easilly customisable and extendable

 ## [Architecture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture.markdown)
 - [Component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture/components.markdown)-based architecture applied across the engine in the form of :
    - LightningComponents for game object behaviors 
    - LightningFragment for fragment, vertex, and geometry shaders
    - ContentComponents for [Resources](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture/resources.markdown) meta data 

 ## [Graphics](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/graphics.markdown)
 - Fully modifiable and scriptable rendering pipeline
    - With a [physically-based renderer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/graphics/physically_based_rendering.markdown) provided as the default renderer
 - Dedicated render thread
 - SSAO and Bloom

 ## [Physics](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics.markdown)
 - Custom-built, three-dimensional, constraint-based physics engine
 - Regions that can apply both pre-defined and user-defined [PhysicsEffects](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicseffectsandregions.markdown)
 - Robust, customizable [joint system](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/joints.markdown)

 ## [Audio](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio.markdown)
 - Scripted, [node-based](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode.markdown) DST system
 - 3D sound [positioning](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundemitter.markdown) and [attenuation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundattenuator.markdown)

 ## [Lightning](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/lightning_in_plasma.markdown)
 - High-level scripting and shader language


 # Learning the Plasma Engine
Not all users have the same level of experience, with the Plasma Engine or game engines in general. The following guidelines and recommendations provide recommendations for any level of user with different types of background and experience to become productive in Plasma.

 ## Novice Users
So you have never made a game or even programmed before. No problem! We have a sequence of [ tutorials ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/tutorials.markdown) and [ manual ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown) pages that will instruct you in the basics of both Plasma and game programming in general. We suggest users of this level take the following steps to get started.

 ### New To Everything
 - The [standard tutorial sequence](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/tutorials/tutorial_sequences.markdown) will get you up and interacting with the Editor in the shortest amount of time possible. It is an excellent place to start if you want to dive right in.
 - The PlasmaManual contains a wealth of information If you find yourself curious about about a certain [major engine system](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown), [imported or generated resource](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture/resources.markdown), or concept, such as  [components](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture/components.markdown), [Events](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/scripting/eventsandconnections.markdown), or [archetypes](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture/archetypes.markdown).

 ### Some Prior Game Engine Experience
 - If you have some experience with another game engine, you may wish to create a new project and start playing around. The best way to learn is to do and experiment.
 - If you find yourself stuck or curious about a part of the engine you're unfamiliar with, check out the [PlasmaManual](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown) for detailed coverage of the major systems,  individual elements, and concepts unique to the Plasma Engine. 

Once you've mastered the basics taught in the Basics and Beginner  [tutorial_sequences](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/tutorials/tutorial_sequences.markdown) and feel comfortable with the Editor UI and essential features, continue down to Intermediate Users.

 ## Intermediate Users
If you have some experience making games and programming, you will be able to pick things up fairly quickly.

 - Start with the [lightning_in_plasma](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/lightning_in_plasma.markdown). You will probably want to jump into scripting pretty quickly.
 - Read the [plasmamanual](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown) starting with the [editor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor.markdown), [architecture](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/architecture.markdown), and [gameplay](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/gameplay.markdown) sections.
 - Browse [physics](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics.markdown), [editor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/editor.markdown) and [audio](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio.markdown) sections for topics that are applicable to your project.
 - Read the remaining [plasmamanual](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown) sections at your own pace.
 - If you are not fully confident in your ability to start operating in the engine, try out some [tutorials](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/tutorials.markdown).
 - Remember that you can always look things up in the [code_reference](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference.markdown)
 
  ## Advanced Users
Practice, Practice and Practice.

- Keep experimenting and creating
- Refer back to the  [plasmamanual](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual.markdown) when you have questions
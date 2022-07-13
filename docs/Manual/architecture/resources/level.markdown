A level is resource that stores a set of objects which will then be created later when the level is loaded. Levels can be loaded into a space in order to create all objects saved to the resource. Levels can be edited using several tools, especially those found via the [Editor UI](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorui.markdown).
# Levels

## Using Levels
### Creating a Level
A new level can be added by using the Add command ([Command](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorcommands/commands.markdown) : [Add](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/command_reference.markdown#add) or clicking on the Add button button) followed by selecting Level drop-down menu. The newly-created level will open in the Level Window and allow for the manipulation of objects to build game levels. At creation the level will only have the default objects inside it: `LevelSettings` and a few other object from the level template you select.


 - The [LevelSettings](https://plasmaengine.github.io/PlasmaDocs/Manual/architecture/objects/levelsettings.markdown) object is a cog that has a single unique instance per level that cannot be deleted or duplicated. It has several components attached in order to run various effects in the level, such as gravity.

The background grid will also be turned on. The grid is there to help place objects within the level editor but will not be visible during gameplay, and can be turned on and off by using the toolbar in the top left corner of the Level Window.



![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/levelTools.PNG) *The collapsible toolbar has a few buttons for altering the view.*



| Buttons                             | Purpose |
|-------------------------------------|---------------------------------------------|
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/2DToggle.png) ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/3DToggle.png) | Toggles between 2D & 3D camera controls.    |
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/OrthographicToggle.png) ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/PerspectiveToggle.png) | Toggles the editor camera's rendering mode between Orthographic and Perspective Projection. |
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/GridOn.PNG) ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/GridOff.PNG) | Toggles the grid line visuals in the editor. |
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/DebugViews.png) | With the debug views option you can preview diffrent rendering buffers, this is useful for debugging issues with materials.  |
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/CameraOptions.png)  | With the camera options you can either reset the editor camera to its default settings, or align a selected camera with the editor's camera.  |
| ![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/Speed.png)  | This option allows you to change the speed of the editor movement.  |

## Levels vs. Spaces
While levels are resources that store object data to later be loaded, spaces are where those objects are placed upon creation. This allows multiple spaces to load multiple levels at once, which is used to create HUD or UI elements, or to pause the main game while still allowing pause menus to function properly. 

```
// The level made with all the Pause Menu UI elements
[Property]
var PauseLevel : Level;

// A property to hold a Space archetype used to create the Pause level
[Property]
var PauseSpaceArchetype : Archetype;

// A variable used as a reference for the Space holding the pause menu
var PauseSpace : Space = null;

function Initialize(init : CogInitializer)
{
}

function Pause()
{
    // Create a new named Space for the Pause Menu
    this.PauseSpace = this.GameSession.CreateNamedSpace("PauseSpace", this.PauseSpaceArchetype);
     // Load the Pause Menu level in the newly created Space
    this.PauseSpace.LoadLevel(this.PauseLevel);
}

function UnPause()
{
    // If the PauseSpace exists, destroy it along with the Pause level
    if (this.PauseSpace != null)
        this.PauseSpace.Destroy();
}
```


This code snippet gives an example of having two levels exist at once. By giving it a `Space` archetype and `level` to load and then calling the `Pause()` function in a LightningScript, it will create a new Space and load the new level without destroying the currently existing one. The `Unpause()` function will do the reverse, and destroy the level and Space. 

# Related Materials
## Manual
- [Editor UI](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorui.markdown)
- [Spaces](https://plasmaengine.github.io/PlasmaDocs/Manual/architecture/objects/spaces.markdown)
- [CamerasViewportsRenderers](https://plasmaengine.github.io/PlasmaDocs/Manual/graphics/camerasviewportsrenderers.markdown)
- [Level Settings](https://plasmaengine.github.io/PlasmaDocs/Manual/architecture/objects/levelsettings.markdown)
 

 
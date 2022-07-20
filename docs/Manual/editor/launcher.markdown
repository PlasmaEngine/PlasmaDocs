# Launcher

This page covers the launcher and its multiple subtabs.

#  [Download the Engine](http://download.plasmaengine.io )

# The Discover Tab


**ADD IMAGE**

The Discover tab is the Launcher's information hub, featuring links to documentation, news, and informative websites.



**ADD IMAGE**


| Link | Description |
| -- | -- |
| [PlasmaHub](https://dev.plasmaengine.io/) | The PlasmaHub homepage |
| [Lightning](https://plasmaengine.github.io/PlasmaDocs/Manual/lightning_in_plasma.markdown) | The Lightning user documentation |
| [ROADMAP](https://dev.plasmaengine.io/project/board/52/) | An overview of current development on Plasma Engine |
| [DOCUMENTATION](https://github.com/PlasmaEngine/PlasmaDocs/blob/master.markdown) | The root documentation page |

# The Projects Tab


**ADD IMAGE**

The Projects tab lets the user create new projects and manage existing ones.

## New Project


**ADD IMAGE** *Project Creation*

### Project Templates
The project templates are `EMPTY 2D PROJECT` and `EMPTY 3D PROJECT`. Both options will result in an empty Plasma project, but with a few differences in settings.


**ADD IMAGE**


**New Project Default Settings by Template**

| **Setting**  | **Description** | `EMPTY 2D PROJECT` | `EMPTY 3D PROJECT` |
|--------------|-----------------|----------------------|----------------------|
| PhysicsSpace **Mode2D** | Default behavior for collision resolution | `true` | `false` |
| EditorCamera | Settings of editor camera | 2D (orthographic projection, etc.) | 3D (perspective projection, etc.) |
| DefaultCamera | Settings of the camera that is placed by default in each new level | 2D (orthographic projection, etc.) | 3D (perspective projection, etc.) |
| GridDraw **Axis** | Perpendicular axis to the grid plane | `ZAxis` | `YAxis` |

NOTE: Even if a game starts with the 2D template, it can still become a 3D game or even just use 3D elements.  The template you choose simply specifies the default settings for certain properties.

### Name and Location
The Name  of the project is required, but the `TAGS field` is optional.  Both are ways of labeling a project so that it can be searched for in the [Recent Projects](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/launcher.markdown#recent-projects) subtab.  TAGS  will parse a comma-delimited list of strings, where each string becomes a seperate tag: `<tag1>, <tag2>, <tag3>`


**ADD IMAGE**


### Version
The version can be selected from here as long as it's installed from the [Builds tab](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/launcher.markdown#the-builds-tab).  Optionally, the latest version can be installed by selecting `the version drop-down  > INSTALL LATEST`


**ADD IMAGE**


## Recent Projects


**ADD IMAGE**


Moving on to projects previously created, by clicking the **Recent** button you will bring up the Recent Projects subtab.
The recent projects tab a list of the latest Plasma projects that were worked on.  The maximum number of recent projects shown can be changed through the `MAX RECENT PROJECTS` in the [Settings tab](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/launcher.markdown#the-settings-tab).

### Project Tiles
Each recent project will show up as a project tile, showing information relating to that project.  There is an option to remove a tile from the project list, by clicking on an X on the bottom right of the tile.


**ADD IMAGE**


### Search Bar
The search bar can be used to filter the project list, by name and by tag.


**ADD IMAGE**

### In a Project Tile
Once a project tile is selected, more information and a launch option are displayed.  Clicking on the **ADD IMAGE** button will open the directory of the project.  The version selector works the same as the one in the [New subtab](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/launcher.markdown#new-project).


**ADD IMAGE**


## Browse Projects
Clicking on the **Browse** subtab will open the systems default explorer to manually find and locate a project.  The expected file type of a project is `.plasmaproj`.

## The Builds Tab


**ADD IMAGE**


The Builds tab features a list of Plasma Engine build versions that are currently installed or available for download.  A new build can be installed by clicking on it's version in the left pane, and finding the **ADD IMAGE** button.  Alternatively, an installed version will have a **ADD IMAGE** button for uninstalling.

(WARNING)**Why Choose a Different Build?**
While it may seem unnecessary initially, having access to earlier builds of the engine can be beneficial.  Changing the version between project launches can make a project unplayable, unlaunchable, or otherwise broken.  One solution is to fix the project as the latest engine version changes, but time may not permit this.  The quicker more reliable solution is to retain the version of the last working build.



**ADD IMAGE**


WARNING:
Any number of builds can be installed and stored at once, but each build installed takes up around `300` MB of disk space.

## The Settings Tab


**ADD IMAGE**


The settings tab has a number of different properties about how the Launcher itself behaves.



**ADD IMAGE**


`PROJECT SETTINGS`: Choose whether to launch the launcher or the engine when a plasma project is opened.

`DEFAULT PROJECT LOCATION`: Where projects are saved.
`DEFAULT DOWNLOAD LOCATION`: Where builds are saved.

`MAX RECENT PROJECTS`: The most project tiles that can show up on the [Recent Projects](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/launcher.markdown#recent-projects) subtab.
`AUTO CHECK FOR MAJOR UPDATES`:  Check for updates
`SHOW DEVELOPMENT BUILDS`: This shows more recent and potentially unstable builds.
`SHOW EXPERIMENTAL BRANCHES`:  This shows builds from other branches of the Plasma Engine repository.

`Revert to default`:  Restores the launcher to its default settings.

## Related Materials
### Manual
- [launchernewproject](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorcommands/launchernewproject.markdown) 

 

# Plasma Launcher

## Prerequisite
- Have the launcher installed

## Learning Objectives


- Launcher tabs and sections
- Creating new projects
- Build installation


# The Discover Tab

The Discover tab is the Launcher's information hub. It features a number of useful links to informative websites such as the Documentation page and Plasma website. It also contains Development updates posted by the Plasma team so you can stay up to date and informed about the latest news in from the Plasma ecosystem.

The **Plasma Website** link opens the Plasma Engine open-source development site.

The **Documentation** link opens the Plasma Engine documentation website.

The **Roadmap** link takes you to the public development roadmap for Plasma.

The **Discord** link connects you to the Plasma discord where you can get question answered and discus the engine.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/LauncherDiscover.PNG)

# The Projects Tab

## *New Project*

| New Project Default Settings by Template |--|--|--|
|--|--|--|--|
| **Setting**  | **Description**| **EMPTY 2D PROJECT** | **EMPTY 3D PROJECT**|
|[ PhysicsSpace ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/physicsspace.markdown) {nav icon=check-square-o, name=Mode2D}| Default behavior for collision resolution| `true`|`false`|
|EditorCamera|Settings of editor camera|2D (orthographic, etc...)|3D (perspective, etc...)|
|Default Camera|Settings of the camera that is placed by default in each new level|2D (orthographic, etc...)|3D (perspective, etc...)|
|GridDraw Axis|Perpendicular axis to the grid plane|`ZAxis`|`YAxis`|

(NOTE) **Remember**, even if you start with the 2D template, **you can still use 3D elements and concepts in your game**, and vice versa. The template you choose simply specifies the default settings for certain properties.

1. Choose a template to start with, Either 2D or 3D

2. Type a name for the project in the **Name** field. (You will be notified if a project by the same name already exists in the folder specified in the **Location** field.)

3. Specify where the project should be created in the **Location** field. The default path for new projects can be changed in The Settings Tab. You can use the **Open Path** button next to the field to browse to a desired folder in your operating system's Folder Selection dialog.

4. Optionally, you may give the project *tags* by typing them, separated by commas, in the **Tags** field. Tags are just bits of text that can be used as keywords when searching for projects in the Recent Projects subtab.

5. Specify which Plasma Engine build version that you want to use to create the project in the **Build** popup menu.

6. When you are ready, click the **Create Project** button. This will create a
  folder with the project name in the specified location containing the project
  file and Content folder. 
  
![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/NewProject.PNG)

 ##  *Recent Projects*


Here, you will see a list of the latest projects that you have worked on. From here you can open project along with change there engine versions, Delete the projects, Rename project and go to there location on the computer.


![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/RecentProjects.PNG)

1. Each recently-used project appears here, with its name and modified date shown next to a thumbnail screenshot.
2. You may use the **Search** field to search through your recent projects, either by name or by tags.
3. When you mouse over a recent project, its **Remove** button will appear, which you may use to remove the project from the Recent Projects subtab.
 - Removing a project in this way only removes it from this list. It does not delete the project from your computer.



*The Recent Projects, with a project selected*


1. To open the project, click the **Launch Project** button.
2. You may choose which installed Plasma Engine build version you wish to open the project in by selecting the desired build from the **Build** popup menu.
3. Clicking the **Open Path** button will open the project folder in your operating system.
4. To return to the list of recent projects, click the **Back** button.


 ##  *Browse Projects*


Click Browse button to find a Plasma project through your operating system's Open dialog.


 #  The Builds Tab


The Builds tab features a list of Plasma Engine builds that are installed on your computer or available for download. From here you can install desired engine versions along with removing any undesired versions. You are also able to see the release notes for each version when it is selected.



![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/Builds.PNG)


1. Each build is listed in the **Build List** section of the builds tab, with its build number, release date, and tags.

2. Further information on the selected build can be found in the **Details** pane.

3. You may use the **Search** field to search through the Build List, either by build number or by tags.

4. Click the **Install Build** button to download and install the selected build.

5. Click the **Uninstall** button to remove the selected build from your computer.

NOTE: You may have **any number of different builds** installed simultaneously.

 

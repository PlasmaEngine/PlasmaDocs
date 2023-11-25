 `Component` `Engine`



(NOTE) Project component store primary data for a project. Projects are separate games with their own content and settings.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#projectsettings-void)|[ AutoTakeProjectScreenshot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#autotakeprojectscreensho)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ ContentFolder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#contentfolder-plasma-engin)| | |
| |[ EditorContentFolder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#editorcontentfolder-plasma)| | |
| |[ ProjectFolder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#projectfolder-plasma-engin)| | |
| |[ ProjectName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#projectname-plasma-engine)| | |
| |[ ProjectOwner](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/projectsettings.md#projectowner-plasma-engine)| | |


 #  Properties


---  
 #  AutoTakeProjectScreenshot : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var AutoTakeProjectScreenshot : Boolean


---  
 #  ContentFolder : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the path to the generated content folder for this project.
> ``` lang=cpp, name=Lightning
> var ContentFolder : String


---  
 #  EditorContentFolder : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the path to the content folder containing editor specific content (screen shot, editor settings, etc...).
> ``` lang=cpp, name=Lightning
> var EditorContentFolder : String


---  
 #  ProjectFolder : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the path to the folder containing this project.
> ``` lang=cpp, name=Lightning
> var ProjectFolder : String


---  
 #  ProjectName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> Returns the Project's Name.
> ``` lang=cpp, name=Lightning
> var ProjectName : String


---  
 #  ProjectOwner : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> 
> ``` lang=cpp, name=Lightning
> var ProjectOwner : String


---  
 #  Methods


---  
 #  ProjectSettings : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ProjectSettings()
> ``` 


---  
 #  ProjectSettings : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ProjectSettings()
> ``` 


---  
 

 
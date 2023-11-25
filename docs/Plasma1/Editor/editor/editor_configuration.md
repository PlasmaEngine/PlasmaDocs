# Editor Configuration

The Plasma Editor has a number of configuration settings that can be modified within the editor, such as text editor preferences.

#  Selecting the EditorConfig Object

To modify the editor's settings, first select the EditorConfig object:

- In the `Level Window`
- Press `Shift + E`

**Or**

- Click `Select  > Select Editor Config`

#  EditorConfig Components

Components found on EditorConfig object are unique to it, and cannot be attached to other objects.



**ADD IMAGE**

*`Properties Window` of EditorConfig object*


##  MainConfig

The [ MainConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mainconfig.md) component shows details about the current version of the editor. *Its fields are read-only.*



**ADD IMAGE**


*The [ MainConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mainconfig.md) component*


##  ContentConfig

The **ContentConfig** component contains settings controlling the loading of additional content libraries when using the Plasma Editor.

- *This component is #deprecated and is not accessible from within the Plasma Editor. It currently exists for #legacy purposes.*

##  TextEditorConfig

The [ TextEditorConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texteditorconfig.md) component allows the user to view and modify various settings of Plasma's text editor.

###  TabWidth
The text editor may be configured to insert either two or four spaces when the `Tab` key is pressed.


**ADD IMAGE** **ADD IMAGE**

*Left: `TwoSpaces`, Right: `FourSpaces`*
 

###  ShowWhiteSpace
If this is `true`, whitespace characters are shown as little dots.


**ADD IMAGE** **ADD IMAGE**


*Left: `true`, Right: `false`*


###  LineNumbers
If this is `true`, Lightning files will display their line numbers in the gutter.


**ADD IMAGE** **ADD IMAGE**


*Left: `true`, Right: `false`*


###  CodeFolding
**Code folding** is a common feature of code editors that allows the user to hide code that they don't want to see at the moment. In the Plasma Editor, with code folding enabled, any paired set of curly braces may be collapsed by clicking its toggle button in the editor. If code folding is disabled, these controls will be hidden, and the code folding section of the gutter will be collapsed.


**ADD IMAGE**


###  ConfidentAutoCompleteOnSymbols
If this is `true`, code completion suggestions can be accepted and inserted into the file by typing a symbol character, such as a period or a parenthesis.


**ADD IMAGE**


###  FontSize
This defines the initial font size used for text files when they are opened in the editor. This can be changed on a per-file basis by pressing `Control + +` and `Control + -`, or by holding `Control` and using the scroll wheel. Changes made to a file's font size in this manner are overwritten by the FontSize  property when that file is closed.

##  EditorSettings

The [editorsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/editorsettings.md) component allows the user to view and modify various general editor settings.

WARNING: Some of the settings in this component should not be modified by the user, as noted below.

###  ViewCube
If this is `true`, the view cube is visible in the upper-right corner of the `Level Window`.

###  ViewCubeSize
This defines the size of the view cube, if it is visible.


**ADD IMAGE**

###  ScriptReloadGame
This defines what happens in the event that a script is modified while the game is running in the editor.
- *This property is deprecated and should not be changed. It currently exists for legacy purposes.*

###  AutoUpdateContentChanges
This defines what happens in the event that an open project's content library is modified while the editor is running.
- *This property is deprecated and should not be changed. It currently exists for legacy purposes.*

##  EditorConfig

The **EditorConfig** component contains settings that define which project and which level from that project are opened when the editor is opened. It has no editable properties from within the editor because it is not intended to be modified by the user.

NOTE: The data from EditorConfig object is read from and written to a config file on the user's hard drive, in the `Documents  > PlasmaEditor` folder. This includes data that cannot be modified from within the Plasma Editor. An experienced user may make changes to the config file directly. While this is not strictly forbidden, it is generally not recommended. The config file is called {nav icon=file, name=ConfigurationVX.data}, where *X* is a number, with more recent config files using larger numbers. Later versions of the engine may use the same config file, or they may create a new one with a larger number. In general, the latest engine version will always use the latest config file.

#  Related Materials

##  Manual
- [Project Configuration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/project_configuration.md)
- [ Tab Completion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/editor/texteditor/tab_completion.md)

##  Reference
- [ MainConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mainconfig.md)
- [ TextEditorConfig](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/texteditorconfig.md)
- [editorsettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/editorsettings.md)
- [ TabWidth](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#tabwidth) 

 
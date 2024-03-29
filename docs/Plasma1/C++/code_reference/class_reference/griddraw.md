 `Component` `Editor`



(NOTE) A component used for drawing a grid.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#griddraw-void)|[ Active](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#active-plasma-engine-docum)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
| |[ AlwaysDrawInEditor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#alwaysdrawineditor-plasma)| | |
| |[ Axis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#axis-plasma-engine-documen)| | |
| |[ CellSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#cellsize-plasma-engine-doc)| | |
| |[ DrawAxisOrigins](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#drawaxisorigins-plasma-eng)| | |
| |[ DrawInGame](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#drawingame-plasma-engine-d)| | |
| |[ FollowEditorCamera](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#followeditorcamera-plasma)| | |
| |[ GridColor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#gridcolor-plasma-engine-do)| | |
| |[ GridHighlight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#gridhighlight-plasma-engin)| | |
| |[ HalfCellOffset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#halfcelloffset-plasma-engi)| | |
| |[ HighlightInterval](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#highlightinterval-plasma-e)| | |
| |[ Lines](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/griddraw.md#lines-plasma-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> 
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AlwaysDrawInEditor : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Always draw the grid in editor (not just when it's selected)
> ``` lang=cpp, name=Lightning
> var AlwaysDrawInEditor : Boolean


---  
 #  Axis : [AxisDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#axisdirection)

> 
> ``` lang=cpp, name=Lightning
> var Axis : AxisDirection


---  
 #  CellSize : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The deltas in the grid (how far apart we draw grid lines)
> ``` lang=cpp, name=Lightning
> var CellSize : Real


---  
 #  DrawAxisOrigins : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Changes the line color to.
> ``` lang=cpp, name=Lightning
> var DrawAxisOrigins : Boolean


---  
 #  DrawInGame : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Draw the grid in the game.
> ``` lang=cpp, name=Lightning
> var DrawInGame : Boolean


---  
 #  FollowEditorCamera : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Move with the editor camera?
> ``` lang=cpp, name=Lightning
> var FollowEditorCamera : Boolean


---  
 #  GridColor : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> Color of grid lines.
> ``` lang=cpp, name=Lightning
> var GridColor : Real4


---  
 #  GridHighlight : [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)

> 
> ``` lang=cpp, name=Lightning
> var GridHighlight : Real4


---  
 #  HalfCellOffset : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Is the grid offset by half a unit?
> ``` lang=cpp, name=Lightning
> var HalfCellOffset : Boolean


---  
 #  HighlightInterval : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> How often should cells be activated.
> ``` lang=cpp, name=Lightning
> var HighlightInterval : Integer


---  
 #  Lines : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> The number of lines to draw.
> ``` lang=cpp, name=Lightning
> var Lines : Integer


---  
 #  Methods


---  
 #  GridDraw : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function GridDraw()
> ``` 


---  
 

 
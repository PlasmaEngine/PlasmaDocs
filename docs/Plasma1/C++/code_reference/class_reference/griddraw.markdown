 `Component` `Editor`



(NOTE) A component used for drawing a grid.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#griddraw-void)|[ Active](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#active-plasma-engine-docum)|[component](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/component.markdown)| |
| |[ AlwaysDrawInEditor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#alwaysdrawineditor-plasma)| | |
| |[ Axis](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#axis-plasma-engine-documen)| | |
| |[ CellSize](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#cellsize-plasma-engine-doc)| | |
| |[ DrawAxisOrigins](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#drawaxisorigins-plasma-eng)| | |
| |[ DrawInGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#drawingame-plasma-engine-d)| | |
| |[ FollowEditorCamera](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#followeditorcamera-plasma)| | |
| |[ GridColor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#gridcolor-plasma-engine-do)| | |
| |[ GridHighlight](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#gridhighlight-plasma-engin)| | |
| |[ HalfCellOffset](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#halfcelloffset-plasma-engi)| | |
| |[ HighlightInterval](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#highlightinterval-plasma-e)| | |
| |[ Lines](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/griddraw.markdown#lines-plasma-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> ``` lang=cpp, name=Lightning
> var Active : Boolean


---  
 #  AlwaysDrawInEditor : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Always draw the grid in editor (not just when it's selected)
> ``` lang=cpp, name=Lightning
> var AlwaysDrawInEditor : Boolean


---  
 #  Axis : [AxisDirection](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#axisdirection)

> 
> ``` lang=cpp, name=Lightning
> var Axis : AxisDirection


---  
 #  CellSize : [real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown)

> The deltas in the grid (how far apart we draw grid lines)
> ``` lang=cpp, name=Lightning
> var CellSize : Real


---  
 #  DrawAxisOrigins : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Changes the line color to.
> ``` lang=cpp, name=Lightning
> var DrawAxisOrigins : Boolean


---  
 #  DrawInGame : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Draw the grid in the game.
> ``` lang=cpp, name=Lightning
> var DrawInGame : Boolean


---  
 #  FollowEditorCamera : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Move with the editor camera?
> ``` lang=cpp, name=Lightning
> var FollowEditorCamera : Boolean


---  
 #  GridColor : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> Color of grid lines.
> ``` lang=cpp, name=Lightning
> var GridColor : Real4


---  
 #  GridHighlight : [real4](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real4.markdown)

> 
> ``` lang=cpp, name=Lightning
> var GridHighlight : Real4


---  
 #  HalfCellOffset : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Is the grid offset by half a unit?
> ``` lang=cpp, name=Lightning
> var HalfCellOffset : Boolean


---  
 #  HighlightInterval : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> How often should cells be activated.
> ``` lang=cpp, name=Lightning
> var HighlightInterval : Integer


---  
 #  Lines : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

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
 

 
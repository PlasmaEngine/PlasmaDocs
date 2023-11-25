 `Component` `Graphics`



(NOTE) Text that is rendered from a texture atlas in the same way that Sprites are.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCharacterPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#getcharacterposition-zer)|[ Font](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#font-plasma-engine-documen)|[basesprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basesprite.md)| |
|[ MeasureGivenText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#measuregiventext-plasma-en)|[ FontSize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#fontsize-plasma-engine-doc)| | |
|[ MeasureText](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#measuretext-plasma-engine)|[ PixelsPerUnit](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#pixelsperunit-plasma-engin)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#spritetext-void)|[ Text](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#text-plasma-engine-documen)| | |
| |[ TextAlign](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritetext.md#textalign-plasma-engine-do)| | |


 #  Properties


---  
 #  Font : [font](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/font.md)

> Font used to display the text.
> ``` lang=cpp, name=Lightning
> var Font : Font


---  
 #  FontSize : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Size that the font will be rastered at to a texture atlas.
> ``` lang=cpp, name=Lightning
> var FontSize : Integer


---  
 #  PixelsPerUnit : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Number of pixels of the font size that map to one world space unit.
> ``` lang=cpp, name=Lightning
> var PixelsPerUnit : Real


---  
 #  Text : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Text to display.
> ``` lang=cpp, name=Lightning
> var Text : String


---  
 #  TextAlign : [TextAlign](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#textalign)

> How to position the text about the objects origin.
> ``` lang=cpp, name=Lightning
> var TextAlign : TextAlign


---  
 #  Methods


---  
 #  GetCharacterPosition : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Get the position in world space of a character by index.
> |Name|Type|Description|
> |---|---|---|
> |characterIndex|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetCharacterPosition(characterIndex : Integer) : Real3
> ``` 


---  
 #  MeasureGivenText : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Get the effective size in world space that the SpriteText would be if this was its text.
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function MeasureGivenText(text : String) : Real2
> ``` 


---  
 #  MeasureText : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)

> Get the effective size in world space of the current text.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function MeasureText() : Real2
> ``` 


---  
 #  SpriteText : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function SpriteText()
> ``` 


---  
 

 
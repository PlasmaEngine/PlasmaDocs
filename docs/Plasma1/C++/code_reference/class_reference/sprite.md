 `Component` `Graphics`



(NOTE) A generated quad that addresses atlased image data for efficient frame-based animations and batched rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#sprite-void)|[ AnimationActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#animationactive-plasma-eng)|[basesprite](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/basesprite.md)| |
| |[ AnimationSpeed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#animationspeed-plasma-engi)| | |
| |[ CurrentFrame](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#currentframe-plasma-engine)| | |
| |[ FlipX](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#flipx-plasma-engine-docume)| | |
| |[ FlipY](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#flipy-plasma-engine-docume)| | |
| |[ SpriteSource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#spritesource-plasma-engine)| | |
| |[ StartFrame](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/sprite.md#startframe-plasma-engine-d)| | |


 #  Properties


---  
 #  AnimationActive : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If the Sprite animation should be playing on logic update, paused if false.
> ``` lang=cpp, name=Lightning
> var AnimationActive : Boolean


---  
 #  AnimationSpeed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Scalar to the amount of time passed used to advance frames of animation.
> ``` lang=cpp, name=Lightning
> var AnimationSpeed : Real


---  
 #  CurrentFrame : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Index of the frame the animation is currently on.
> ``` lang=cpp, name=Lightning
> var CurrentFrame : Integer


---  
 #  FlipX : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Flips the X axis of the Sprite's image (left/right).
> ``` lang=cpp, name=Lightning
> var FlipX : Boolean


---  
 #  FlipY : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Flips the Y axis of the Sprite's image (top/bottom).
> ``` lang=cpp, name=Lightning
> var FlipY : Boolean


---  
 #  SpriteSource : [spritesource](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/spritesource.md)

> The resource defining one or more image sequences used for frame-based animation.
> ``` lang=cpp, name=Lightning
> var SpriteSource : SpriteSource


---  
 #  StartFrame : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Index of the frame to start the animation on when the object is initialized, 0-based.
> ``` lang=cpp, name=Lightning
> var StartFrame : Integer


---  
 #  Methods


---  
 #  Sprite : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Sprite()
> ``` 


---  
 

 
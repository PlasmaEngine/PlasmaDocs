 `Graphics`

(NOTE) Interface for rendering output. Texture data is managed and recycled by the engine.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Release](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/rendertarget.markdown#release-void)|[ Texture](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/rendertarget.markdown#texture-plasma-engine-docu)|[safeid32](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/safeid32.markdown)| |


 #  Properties


---  
 #  Texture : [texture](https://github.com/dragonCASTjosh/PlasmaDocs/blob/master/code_reference/class_reference/texture.markdown)

 `read-only`

> Texture that is rendered to. Can be used as shader input to a separate rendering operation.
> ``` lang=cpp, name=Lightning
> var Texture : Texture


---  
 #  Methods


---  
 #  Release : Void

> Allows the managed Texture being referenced by this RenderTarget to be reused by the renderer if the same specifications are requested again. Also deletes this RenderTarget.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Release()
> ``` 


---  
 

 
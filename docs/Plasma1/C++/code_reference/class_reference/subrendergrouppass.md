 `Graphics`

(NOTE) Interface used to define unique render settings for a base RenderGroup and its sub RenderGroups.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddSubSettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subrendergrouppass.md#addsubsettings-void)| |[safeid32](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32.md)| |
|[ ExcludeSubRenderGroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subrendergrouppass.md#excludesubrendergroup-vo)| | | |
|[ Reset](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subrendergrouppass.md#reset-void)| | | |
|[ SetDefaultSettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/subrendergrouppass.md#setdefaultsettings-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  AddSubSettings : Void

> Define the settings to use for a specific RenderGroup. Given RenderGroup must be a child of the base RenderGroup, or the base itself, that this was initialized with.
> |Name|Type|Description|
> |---|---|---|
> |subSettings|[rendersettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.md)| |
> |subGroup|[rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)| |
> |subPass|[materialblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/materialblock.md)| |
> ``` lang=cpp, name=Lightning
> function AddSubSettings(subSettings : RenderSettings, subGroup : RenderGroup, subPass : MaterialBlock)
> ``` 


---  
 #  ExcludeSubRenderGroup : Void

> Explicitely exclude a RenderGroup from rendering when there are default settings. Given RenderGroup must be a child of the base RenderGroup, or the base itself, that this was initialized with.
> |Name|Type|Description|
> |---|---|---|
> |subGroup|[rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Lightning
> function ExcludeSubRenderGroup(subGroup : RenderGroup)
> ``` 


---  
 #  Reset : Void

> Resets interface back to the initial creation state with a given base RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |baseRenderGroup|[rendergroup](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Lightning
> function Reset(baseRenderGroup : RenderGroup)
> ``` 


---  
 #  SetDefaultSettings : Void

> Settings to use for the base or all sub RenderGroups that do not have specified settings. Without defaults, the base or any sub RenderGroup without settings will not render.
> |Name|Type|Description|
> |---|---|---|
> |defaultSettings|[rendersettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/rendersettings.md)| |
> |defaultPass|[materialblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/materialblock.md)| |
> ``` lang=cpp, name=Lightning
> function SetDefaultSettings(defaultSettings : RenderSettings, defaultPass : MaterialBlock)
> ``` 


---  
 

 
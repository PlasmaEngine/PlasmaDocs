 `Physics`

(NOTE) An array interface to the cog paths of wheels that this car uses. This array is read-only.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/carwheelarray.markdown#get-plasma-engine-document)|[ Count](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/carwheelarray.markdown#count-plasma-engine-docume)|[safeid32object](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/safeid32object.markdown)| |


 #  Properties


---  
 #  Count : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> How many wheels this car owns.
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  Methods


---  
 #  Get : [cog](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/cog.markdown)

> Get the cog for a wheel by index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Get(index : Integer) : Cog
> ``` 


---  
 

 
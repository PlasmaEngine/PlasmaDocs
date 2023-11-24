 `Engine`

(NOTE) A Joystick is associated with a hardware joystick, and provides the ability to query axes and buttons.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Calibrating](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#calibrating-plasma-engine)|[ AxisCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#axiscount-plasma-engine-do)|[eventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/eventobject.markdown)| |
|[ EndCalibration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#endcalibration-void)|[ ButtonCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#buttoncount-plasma-engine)| | |
|[ GetAxisIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#getaxisindex-plasma-engine)|[ DisabledValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#disabledvalue-plasma-engin)| | |
|[ GetAxisName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#getaxisname-plasma-engine)|[ IsActive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#isactive-plasma-engine-doc)| | |
|[ GetAxisValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#getaxisvalue-plasma-engine)|[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#name-plasma-engine-documen)| | |
|[ GetAxisValueByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#getaxisvaluebyname-plasma)| | | |
|[ GetButtonValue](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#getbuttonvalue-plasma-engi)| | | |
|[ LoadInputMapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#loadinputmapping-void)| | | |
|[ SaveInputMapping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#saveinputmapping-void)| | | |
|[ StartCalibration](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/joystick.markdown#startcalibration-void)| | | |


 #  Properties


---  
 #  AxisCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var AxisCount : Integer


---  
 #  ButtonCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Get the number of buttons or axes.
> ``` lang=cpp, name=Lightning
> var ButtonCount : Integer


---  
 #  DisabledValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only` `static`

> A value that means a joystick axis is invalid. For example when a HAT-switch is not pressed down, it will return this value.
> ``` lang=cpp, name=Lightning
> var DisabledValue : Real


---  
 #  IsActive : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

 `read-only`

> Gets whether or not the joystick is active.
> ``` lang=cpp, name=Lightning
> var IsActive : Boolean


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Get the name of the Joystick.
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  Methods


---  
 #  Calibrating : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Calibrating() : Boolean
> ``` 


---  
 #  EndCalibration : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function EndCalibration()
> ``` 


---  
 #  GetAxisIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxisIndex(name : String) : Integer
> ``` 


---  
 #  GetAxisName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxisName(index : Integer) : String
> ``` 


---  
 #  GetAxisValue : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Queries an axes and returns a value between [-1, 1]. The valid range of axes is between 0 and 'GetMaxAxes'. If the axis is not valid, then the value returned is 0. If the axis is disabled, then the value returned is Joystick.DisabledValue.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxisValue(index : Integer) : Real
> ``` 


---  
 #  GetAxisValueByName : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetAxisValueByName(name : String) : Real
> ``` 


---  
 #  GetButtonValue : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Queries a button and returns true if it is down, false if it is up The valid range of buttons is between 0 and 'GetMaxButtons' If the button is not valid, then the value returned is false.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetButtonValue(index : Integer) : Boolean
> ``` 


---  
 #  LoadInputMapping : Void

> Load an input mapping.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function LoadInputMapping(name : String)
> ``` 


---  
 #  SaveInputMapping : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function SaveInputMapping(name : String)
> ``` 


---  
 #  StartCalibration : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StartCalibration()
> ``` 


---  
 

 
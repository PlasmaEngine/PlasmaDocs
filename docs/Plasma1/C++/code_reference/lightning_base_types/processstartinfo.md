 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#processstartinfo-void)|[ ApplicationName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#applicationname-plasma-eng)| | |
| |[ Arguments](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#arguments-plasma-engine-do)| | |
| |[ RedirectStandardError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#redirectstandarderror-ze)| | |
| |[ RedirectStandardInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#redirectstandardinput-ze)| | |
| |[ RedirectStandardOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#redirectstandardoutput-z)| | |
| |[ SearchPath](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#searchpath-plasma-engine-d)| | |
| |[ ShowWindow](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#showwindow-plasma-engine-d)| | |
| |[ WorkingDirectory](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md#workingdirectory-plasma-en)| | |


 #  Properties


---  
 #  ApplicationName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Name of the application to execute. No quoting of this string is necessary.
> ``` lang=cpp, name=Lightning
> var ApplicationName : String


---  
 #  Arguments : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Arguments to pass to the application.
> ``` lang=cpp, name=Lightning
> var Arguments : String


---  
 #  RedirectStandardError : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not we should redirect the Standard Error of the process for capturing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardError : Boolean


---  
 #  RedirectStandardInput : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not we should redirect the Standard Input of the process for writing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardInput : Boolean


---  
 #  RedirectStandardOutput : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not we should redirect the Standard Output of the process for capturing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardOutput : Boolean


---  
 #  SearchPath : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not we should search the path for the application.
> ``` lang=cpp, name=Lightning
> var SearchPath : Boolean


---  
 #  ShowWindow : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Whether or not the window of the launched application should be shown.
> ``` lang=cpp, name=Lightning
> var ShowWindow : Boolean


---  
 #  WorkingDirectory : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> The working directory for the process to start with. No quoting of this string is necessary.
> ``` lang=cpp, name=Lightning
> var WorkingDirectory : String


---  
 #  Methods


---  
 #  ProcessStartInfo : Void

 `constructor`

> Class used to set up parameters before launching a process.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ProcessStartInfo()
> ``` 


---  
 

 
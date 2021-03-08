 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#processstartinfo-void)|[ ApplicationName](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#applicationname-plasma-eng)| | |
| |[ Arguments](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#arguments-plasma-engine-do)| | |
| |[ RedirectStandardError](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#redirectstandarderror-ze)| | |
| |[ RedirectStandardInput](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#redirectstandardinput-ze)| | |
| |[ RedirectStandardOutput](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#redirectstandardoutput-z)| | |
| |[ SearchPath](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#searchpath-plasma-engine-d)| | |
| |[ ShowWindow](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#showwindow-plasma-engine-d)| | |
| |[ WorkingDirectory](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/processstartinfo.markdown#workingdirectory-plasma-en)| | |


 #  Properties


---  
 #  ApplicationName : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> Name of the application to execute. No quoting of this string is necessary.
> ``` lang=cpp, name=Lightning
> var ApplicationName : String


---  
 #  Arguments : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

> Arguments to pass to the application.
> ``` lang=cpp, name=Lightning
> var Arguments : String


---  
 #  RedirectStandardError : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not we should redirect the Standard Error of the process for capturing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardError : Boolean


---  
 #  RedirectStandardInput : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not we should redirect the Standard Input of the process for writing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardInput : Boolean


---  
 #  RedirectStandardOutput : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not we should redirect the Standard Output of the process for capturing.
> ``` lang=cpp, name=Lightning
> var RedirectStandardOutput : Boolean


---  
 #  SearchPath : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not we should search the path for the application.
> ``` lang=cpp, name=Lightning
> var SearchPath : Boolean


---  
 #  ShowWindow : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Whether or not the window of the launched application should be shown.
> ``` lang=cpp, name=Lightning
> var ShowWindow : Boolean


---  
 #  WorkingDirectory : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

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
 

 
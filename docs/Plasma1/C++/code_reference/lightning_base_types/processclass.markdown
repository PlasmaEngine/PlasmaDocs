 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#close-void)|[ StandardError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#standarderror-plasma-engin)| | |
|[ IsRunning](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#isrunning-plasma-engine-do)|[ StandardInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#standardinput-plasma-engin)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#processclass-void)|[ StandardOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#standardoutput-plasma-engi)| | |
|[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#start-void)| | | |
|[ Terminate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#terminate-void)| | | |
|[ WaitForClose](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processclass.markdown#waitforclose-plasma-engine)| | | |


 #  Properties


---  
 #  StandardError : [filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.markdown)

 `read-only`

> The stream where standard error is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Lightning
> var StandardError : FileStream


---  
 #  StandardInput : [filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.markdown)

 `read-only`

> The stream where standard input is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Lightning
> var StandardInput : FileStream


---  
 #  StandardOutput : [filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.markdown)

 `read-only`

> The stream where standard output is re-directed to. Null if not re-directed
> ``` lang=cpp, name=Lightning
> var StandardOutput : FileStream


---  
 #  Methods


---  
 #  Close : Void

> Closes the wrapper around the process, does not close the process launched.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Close()
> ``` 


---  
 #  IsRunning : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsRunning() : Boolean
> ``` 


---  
 #  ProcessClass : Void

 `constructor`

> Process class used for managing external processes and redirecting their stdio. Used to launch and monitor various external programs.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ProcessClass()
> ``` 


---  
 #  Start : Void

> Begins the execution of another process using the given parameters. 
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.markdown)| |
> ``` lang=cpp, name=Lightning
> function Start(startInfo : ProcessStartInfo)
> ``` 


---  
 #  Terminate : Void

> Attempts to manually shut down the process. This is not safe for the other process or what it's handling.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Terminate()
> ``` 


---  
 #  WaitForClose : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WaitForClose() : Integer
> ``` 


---  
 

 
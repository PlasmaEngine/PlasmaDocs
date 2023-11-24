 `Engine`

(NOTE) A process class that asynchronously reads from standard output and standard error and sends out partial read events. Additionally, the full buffer can be stored for each stream. This makes it possible to read the output of a process in a single-threaded context without having to block on output.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#close-void)|[ StandardError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#standarderror-plasma-engin)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.markdown)| |
|[ Create](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#create-plasma-engine-docum)|[ StandardInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#standardinput-plasma-engin)| | |
|[ IsRunning](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#isrunning-plasma-engine-do)|[ StandardOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#standardoutput-plasma-engi)| | |
|[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#start-plasma-engine-docume)|[ StoreStandardErrorData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#storestandarderrordata-z)| | |
|[ Terminate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#terminate-void)|[ StoreStandardOutputData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#storestandardoutputdata)| | |
|[ WaitForClose](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown#waitforclose-plasma-engine)| | | |


 #  Properties


---  
 #  StandardError : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The cached total results from standard error. Will be empty if StoreStandardErrorData is false.
> ``` lang=cpp, name=Lightning
> var StandardError : String


---  
 #  StandardInput : [filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.markdown)

> 
> ``` lang=cpp, name=Lightning
> var StandardInput : FileStream


---  
 #  StandardOutput : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The cached total results from standard output. Will be empty if StoreStandardOutputData is false.
> ``` lang=cpp, name=Lightning
> var StandardOutput : String


---  
 #  StoreStandardErrorData : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Should the results from standard error be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ``` lang=cpp, name=Lightning
> var StoreStandardErrorData : Boolean


---  
 #  StoreStandardOutputData : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Should the results from standard output be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ``` lang=cpp, name=Lightning
> var StoreStandardOutputData : Boolean


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
 #  Create : [asyncprocess](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.markdown)

 `static`

> Construct a new process. This does not start the process.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Create() : AsyncProcess
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
 #  Start : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Begins the execution of another process using the given parameters. Throws an exception if the process cannot be started.
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.markdown)| |
> ``` lang=cpp, name=Lightning
> function Start(startInfo : ProcessStartInfo) : Boolean
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
 #  WaitForClose : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Waits for a process to close up to a given number of milliseconds. This can take up to 3 * milliseconds due to waiting for the output streams to close.
> |Name|Type|Description|
> |---|---|---|
> |milliseconds|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function WaitForClose(milliseconds : Integer) : Integer
> ``` 


---  
 

 
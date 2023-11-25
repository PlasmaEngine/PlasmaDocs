 `Engine`

(NOTE) A process class that asynchronously reads from standard output and standard error and sends out partial read events. Additionally, the full buffer can be stored for each stream. This makes it possible to read the output of a process in a single-threaded context without having to block on output.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#close-void)|[ StandardError](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#standarderror-plasma-engin)|[referencecountedeventobject](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/referencecountedeventobject.md)| |
|[ Create](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#create-plasma-engine-docum)|[ StandardInput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#standardinput-plasma-engin)| | |
|[ IsRunning](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#isrunning-plasma-engine-do)|[ StandardOutput](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#standardoutput-plasma-engi)| | |
|[ Start](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#start-plasma-engine-docume)|[ StoreStandardErrorData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#storestandarderrordata-z)| | |
|[ Terminate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#terminate-void)|[ StoreStandardOutputData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#storestandardoutputdata)| | |
|[ WaitForClose](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md#waitforclose-plasma-engine)| | | |


 #  Properties


---  
 #  StandardError : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> The cached total results from standard error. Will be empty if StoreStandardErrorData is false.
> ``` lang=cpp, name=Lightning
> var StandardError : String


---  
 #  StandardInput : [filestream](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/filestream.md)

> 
> ``` lang=cpp, name=Lightning
> var StandardInput : FileStream


---  
 #  StandardOutput : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `read-only`

> The cached total results from standard output. Will be empty if StoreStandardOutputData is false.
> ``` lang=cpp, name=Lightning
> var StandardOutput : String


---  
 #  StoreStandardErrorData : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Should the results from standard error be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ``` lang=cpp, name=Lightning
> var StoreStandardErrorData : Boolean


---  
 #  StoreStandardOutputData : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

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
 #  Create : [asyncprocess](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/asyncprocess.md)

 `static`

> Construct a new process. This does not start the process.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Create() : AsyncProcess
> ``` 


---  
 #  IsRunning : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsRunning() : Boolean
> ``` 


---  
 #  Start : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Begins the execution of another process using the given parameters. Throws an exception if the process cannot be started.
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/processstartinfo.md)| |
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
 #  WaitForClose : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WaitForClose() : Integer
> ``` 


---  
 #  WaitForClose : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Waits for a process to close up to a given number of milliseconds. This can take up to 3 * milliseconds due to waiting for the output streams to close.
> |Name|Type|Description|
> |---|---|---|
> |milliseconds|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function WaitForClose(milliseconds : Integer) : Integer
> ``` 


---  
 

 
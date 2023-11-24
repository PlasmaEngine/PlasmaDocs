 `Engine`

(NOTE) A process class that asynchronously reads from standard output and standard error and sends out partial read events. Additionally, the full buffer can be stored for each stream. This makes it possible to read the output of a process in a single-threaded context without having to block on output.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#close-void)|[ StandardError](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#standarderror-plasma-engin)|[referencecountedeventobject](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/referencecountedeventobject.markdown)| |
|[ Create](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#create-plasma-engine-docum)|[ StandardInput](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#standardinput-plasma-engin)| | |
|[ IsRunning](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#isrunning-plasma-engine-do)|[ StandardOutput](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#standardoutput-plasma-engi)| | |
|[ Start](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#start-plasma-engine-docume)|[ StoreStandardErrorData](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#storestandarderrordata-z)| | |
|[ Terminate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#terminate-void)|[ StoreStandardOutputData](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#storestandardoutputdata)| | |
|[ WaitForClose](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown#waitforclose-plasma-engine)| | | |


 #  Properties


---  
 #  StandardError : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The cached total results from standard error. Will be empty if StoreStandardErrorData is false.
> ``` lang=cpp, name=Lightning
> var StandardError : String


---  
 #  StandardInput : [filestream](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/filestream.markdown)

> 
> ``` lang=cpp, name=Lightning
> var StandardInput : FileStream


---  
 #  StandardOutput : [string](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)

 `read-only`

> The cached total results from standard output. Will be empty if StoreStandardOutputData is false.
> ``` lang=cpp, name=Lightning
> var StandardOutput : String


---  
 #  StoreStandardErrorData : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Should the results from standard error be accumulated and stored? If a lot of data is output it may be good to turn this off and use the partial data callback events instead.
> ``` lang=cpp, name=Lightning
> var StoreStandardErrorData : Boolean


---  
 #  StoreStandardOutputData : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

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
 #  Create : [asyncprocess](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/asyncprocess.markdown)

 `static`

> Construct a new process. This does not start the process.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Create() : AsyncProcess
> ``` 


---  
 #  IsRunning : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the process is still running, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsRunning() : Boolean
> ``` 


---  
 #  Start : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> Begins the execution of another process using the given parameters. Throws an exception if the process cannot be started.
> |Name|Type|Description|
> |---|---|---|
> |startInfo|[processstartinfo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/processstartinfo.markdown)| |
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
 #  WaitForClose : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> Waits for a process to close, this will block until the process closes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WaitForClose() : Integer
> ``` 


---  
 #  WaitForClose : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

> Waits for a process to close up to a given number of milliseconds. This can take up to 3 * milliseconds due to waiting for the output streams to close.
> |Name|Type|Description|
> |---|---|---|
> |milliseconds|[integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function WaitForClose(milliseconds : Integer) : Integer
> ``` 


---  
 

 
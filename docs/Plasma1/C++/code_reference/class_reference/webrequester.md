 `Component` `Networking`



(NOTE) A component we can use to facilitate web requests.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#clear-void)|[ Url](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#url-plasma-engine-document)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ Run](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#run-void)| | | |
|[ SetHeader](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#setheader-void)| | | |
|[ SetPostData](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#setpostdata-void)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/webrequester.md#webrequester-void)| | | |


 #  Properties


---  
 #  Url : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Get and set the url that we make requests to.
> ``` lang=cpp, name=Lightning
> var Url : String


---  
 #  Methods


---  
 #  Clear : Void

> Clear headers and post data.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Run : Void

> Run the web request (we should get data back in a WebResponse event).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Run()
> ``` 


---  
 #  SetHeader : Void

> Add a header to the web request .
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |data|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function SetHeader(name : String, data : String)
> ``` 


---  
 #  SetPostData : Void

> Add Post data to the request, this will also change the request to a post request.
> |Name|Type|Description|
> |---|---|---|
> |data|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function SetPostData(data : String)
> ``` 


---  
 #  WebRequester : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function WebRequester()
> ``` 


---  
 

 
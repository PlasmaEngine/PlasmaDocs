 `Component` `Networking`



(NOTE) A component we can use to facilitate web requests.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#clear-void)|[ Url](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#url-plasma-engine-document)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ Run](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#run-void)| | | |
|[ SetHeader](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#setheader-void)| | | |
|[ SetPostData](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#setpostdata-void)| | | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/webrequester.markdown#webrequester-void)| | | |


 #  Properties


---  
 #  Url : [string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)

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
> |name|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |data|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetHeader(name : String, data : String)
> ``` 


---  
 #  SetPostData : Void

> Add Post data to the request, this will also change the request to a post request.
> |Name|Type|Description|
> |---|---|---|
> |data|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
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
 

 
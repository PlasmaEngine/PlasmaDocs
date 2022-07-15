 `Core`(NOTE) Hash Map is an Associative Hashed Container.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#add-void | Add]]|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#all-plasma-engine-document | All]]|HashedContainer<Pair<KeyType,DataType>,PairHashAdapter<Hasher,KeyType,DataType>,Allocator>| |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#clear-void | Clear]]|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#count-plasma-engine-docume | Count]]| | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#contains-plasma-engine-doc | Contains]]|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#keys-plasma-engine-documen | Keys]]| | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#get-plasma-engine-document | Get]]|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#values-plasma-engine-docum | Values]]| | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#getordefault-plasma-engine | GetOrDefault]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#getorerror-plasma-engine-d | GetOrError]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#hashmap-key,value-void | Constructor]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#removeorerror-void | RemoveOrError]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#removeorignore-plasma-engi | RemoveOrIgnore]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#set-plasma-engine-document | Set]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#setorerror-void | SetOrError]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#setorignore-plasma-engine | SetOrIgnore]]| | | |
|[[plasma_engine_documentation/code_reference/lightning_base_types/hashmap_key,value /#setoroverwrite-plasma-engi | SetOrOverwrite]]| | | |


 #  Properties


---  
 #  All : HashMapRange[Key,Value]

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var All : HashMapRange[Key,Value]


---  
 #  Count : [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Count : Integer


---  
 #  Keys : HashMapKeyRange[Key]

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Keys : HashMapKeyRange[Key]


---  
 #  Values : HashMap[Value]

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Values : HashMap[Value]


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function Add( : Key,  : Value)
> ``` 


---  
 #  Clear : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clear()
> ``` 


---  
 #  Contains : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function Contains( : Key) : Boolean
> ``` 


---  
 #  Get : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function Get( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function GetOrDefault( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function GetOrDefault( : Key,  : Value) : Value
> ``` 


---  
 #  GetOrError : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function GetOrError( : Key) : Value
> ``` 


---  
 #  HashMap[Key,Value] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function HashMap[Key,Value]()
> ``` 


---  
 #  RemoveOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function RemoveOrError( : Key)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Lightning
> function RemoveOrIgnore( : Key) : Boolean
> ``` 


---  
 #  Set : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function Set( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function SetOrError( : Key,  : Value)
> ``` 


---  
 #  SetOrIgnore : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function SetOrIgnore( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrOverwrite : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/boolean.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Lightning
> function SetOrOverwrite( : Key,  : Value) : Boolean
> ``` 


---  
 

 
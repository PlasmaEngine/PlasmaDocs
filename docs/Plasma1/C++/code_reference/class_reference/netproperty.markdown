 `Networking`



(NOTE) Network Property. Manages the replication of a single property on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ LastChangeTimePassed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netproperty.markdown#lastchangetimepassed-zer)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.markdown)| |
| |[ LastChangeTimestamp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netproperty.markdown#lastchangetimestamp-plasma)| | |
| |[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netproperty.markdown#name-plasma-engine-documen)| | |
| |[ NetChannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netproperty.markdown#netchannel-plasma-engine-d)| | |
| |[ NetPropertyType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netproperty.markdown#netpropertytype-plasma-eng)| | |


 #  Properties


---  
 #  LastChangeTimePassed : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Elapsed time passed since this net property was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Timestamp indicating when this net property was last changed, else 0.
> ``` lang=cpp, name=Lightning
> var LastChangeTimestamp : Real


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)

 `read-only`

> Net property name.
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  NetChannel : [netchannel](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netchannel.markdown)

 `read-only`

> Operating net channel.
> ``` lang=cpp, name=Lightning
> var NetChannel : NetChannel


---  
 #  NetPropertyType : [netpropertytype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/netpropertytype.markdown)

 `read-only`

> Operating net property type.
> ``` lang=cpp, name=Lightning
> var NetPropertyType : NetPropertyType


---  
 #  Methods


---  
 

 
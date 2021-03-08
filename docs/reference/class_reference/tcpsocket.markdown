 `Networking`

(NOTE) Manages all the client/server/peer connections .

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#close-void)|[ ConnectionCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#connectioncount-plasma-eng)|[eventobject](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/eventobject.markdown)| |
|[ CloseConnection](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#closeconnection-void)|[ IncomingConnectionCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#incomingconnectioncount)| | |
|[ Connect](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#connect-void)|[ OutgoingConnectionCount](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#outgoingconnectioncount)| | |
|[ IsConnected](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#isconnected-plasma-engine)| | | |
|[ Listen](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#listen-plasma-engine-docum)| | | |
|[ SendTo](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#sendto-void)| | | |
|[ SendToAll](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#sendtoall-void)| | | |
|[ SendToAllAndSelf](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#sendtoallandself-void)| | | |
|[ SendToAllExcept](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/tcpsocket.markdown#sendtoallexcept-void)| | | |


 #  Properties


---  
 #  ConnectionCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Get the number of connections we have.
> ``` lang=cpp, name=Lightning
> var ConnectionCount : Integer


---  
 #  IncomingConnectionCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Get the number of incoming connections.
> ``` lang=cpp, name=Lightning
> var IncomingConnectionCount : Integer


---  
 #  OutgoingConnectionCount : [integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)

 `read-only`

> Get the number of outgoing connections.
> ``` lang=cpp, name=Lightning
> var OutgoingConnectionCount : Integer


---  
 #  Methods


---  
 #  Close : Void

> Close all activity (whether listening or connected to a server).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Close()
> ``` 


---  
 #  CloseConnection : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function CloseConnection(index : Integer)
> ``` 


---  
 #  Connect : Void

> Attempt to connect to a host on the given port.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |port|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Connect(host : String, port : Integer)
> ``` 


---  
 #  IsConnected : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Check if we are currently connected to anyone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsConnected() : Boolean
> ``` 


---  
 #  Listen : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |maxConnections|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Listen(port : Integer, maxConnections : Integer) : Boolean
> ``` 


---  
 #  Listen : [boolean](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/boolean.markdown)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |maxConnections|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> |bindTo|[TcpSocketBind](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#tcpsocketbind)| |
> ``` lang=cpp, name=Lightning
> function Listen(port : Integer, maxConnections : Integer, bindTo : TcpSocketBind) : Boolean
> ``` 


---  
 #  SendTo : Void

> Send an event to a specific connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[sendableevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/sendableevent.markdown)| |
> |index|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function SendTo(eventId : String, event : SendableEvent, index : Integer)
> ``` 


---  
 #  SendToAll : Void

> Send an event to all connections.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[sendableevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/sendableevent.markdown)| |
> ``` lang=cpp, name=Lightning
> function SendToAll(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllAndSelf : Void

> Send an event to all connections and dispatch on self.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[sendableevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/sendableevent.markdown)| |
> ``` lang=cpp, name=Lightning
> function SendToAllAndSelf(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllExcept : Void

> Send an event to all connections except a particular connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/string.markdown)| |
> |event|[sendableevent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/sendableevent.markdown)| |
> |exceptIndex|[integer](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function SendToAllExcept(eventId : String, event : SendableEvent, exceptIndex : Integer)
> ``` 


---  
 

 
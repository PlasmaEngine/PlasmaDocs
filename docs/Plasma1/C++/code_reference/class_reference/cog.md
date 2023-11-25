 `Engine`

(NOTE) Game Object Composition class. This class is the foundational object for all dynamic objects in the game world. The Cog is a piece of logical interactive content and the primary mechanism game systems (Graphics, Physics, Etc.) provide functionality and communicate. A Cog can be anything from physical objects like trees, tanks, players to logical objects like teams, triggers, or AI objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddComponentByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#addcomponentbyname-plasma)|[ Actions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#actions-plasma-engine-docu)|Object|[gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md)|
|[ AddComponentByType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#addcomponentbytype-plasma)|[ Archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#archetype-plasma-engine-do)| |[space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)|
|[ AttachTo](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#attachto-plasma-engine-doc)|[ BaseArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#basearchetype-plasma-engin)| | |
|[ AttachToPreserveLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#attachtopreservelocal-ze)|[ ChildCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#childcount-plasma-engine-d)| | |
|[ ClearArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#cleararchetype-void)|[ Children](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#children-plasma-engine-doc)| | |
|[ Clone](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#clone-plasma-engine-docume)|[ ComponentCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#componentcount-plasma-engi)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#cog-void)|[ EditorViewportHidden](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#editorviewporthidden-zer)| | |
|[ DebugDraw](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#debugdraw-void)|[ GameSession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#gamesession-plasma-engine)| | |
|[ Destroy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#destroy-void)|[ LevelSettings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#levelsettings-plasma-engin)| | |
|[ Detach](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#detach-void)|[ Locked](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#locked-plasma-engine-docum)| | |
|[ DetachPreserveLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#detachpreservelocal-void)|[ MarkedForDestruction](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#markedfordestruction-zer)| | |
|[ DispatchDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#dispatchdown-void)|[ Name](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#name-plasma-engine-documen)| | |
|[ DispatchEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#dispatchevent-void)|[ ObjectViewHidden](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#objectviewhidden-plasma-en)| | |
|[ DispatchUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#dispatchup-void)|[ Parent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#parent-plasma-engine-docum)| | |
|[ FindAllChildrenByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findallchildrenbyname-ze)|[ Persistent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#persistent-plasma-engine-d)| | |
|[ FindChildByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findchildbyname-plasma-eng)|[ RuntimeId](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#runtimeid-plasma-engine-do)| | |
|[ FindDirectChildByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#finddirectchildbyname-ze)|[ Space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#space-plasma-engine-docume)| | |
|[ FindNearestArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findnearestarchetype-zer)|[ Transient](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#transient-plasma-engine-do)| | |
|[ FindNextInOrder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findnextinorder-plasma-eng)| | | |
|[ FindNextSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findnextsibling-plasma-eng)| | | |
|[ FindPreviousInOrder](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findpreviousinorder-plasma)| | | |
|[ FindPreviousSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findprevioussibling-plasma)| | | |
|[ FindRoot](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findroot-plasma-engine-doc)| | | |
|[ FindRootArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#findrootarchetype-plasma-e)| | | |
|[ GetComponentByIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#getcomponentbyindex-plasma)| | | |
|[ GetComponentByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#getcomponentbyname-plasma)| | | |
|[ GetComponentIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#getcomponentindex-plasma-e)| | | |
|[ IsAncestorOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#isancestorof-plasma-engine)| | | |
|[ IsDescendant](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#isdescendant-plasma-engine)| | | |
|[ IsDescendantOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#isdescendantof-plasma-engi)| | | |
|[ IsModifiedFromArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#ismodifiedfromarchetype)| | | |
|[ PlaceAfterSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#placeaftersibling-void)| | | |
|[ PlaceBeforeSibling](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#placebeforesibling-void)| | | |
|[ RemoveComponentByName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#removecomponentbyname-ze)| | | |
|[ RemoveComponentByType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#removecomponentbytype-ze)| | | |
|[ ReplaceChild](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#replacechild-void)| | | |
|[ SanitizeName](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#sanitizename-plasma-engine)| | | |
|[ UploadToArchetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md#uploadtoarchetype-void)| | | |


 #  Properties


---  
 #  Actions : [actions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/actions.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Actions : Actions


---  
 #  Archetype : [archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)

> Getter / setter for Archetype.
> ``` lang=cpp, name=Lightning
> var Archetype : Archetype


---  
 #  BaseArchetype : [archetype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/archetype.md)

 `read-only`

> Returns the Archetype our Archetype inherits from.
> ``` lang=cpp, name=Lightning
> var BaseArchetype : Archetype


---  
 #  ChildCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns the amount of children on this Cog. Note that this function has to iterate over all children to calculate the count.
> ``` lang=cpp, name=Lightning
> var ChildCount : Integer


---  
 #  Children : [hierarchylistrange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchylistrange.md)

 `read-only`

> Returns a range of all direct children on this Cog.
> ``` lang=cpp, name=Lightning
> var Children : HierarchyListRange


---  
 #  ComponentCount : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Returns how many Components are on this Cog.
> ``` lang=cpp, name=Lightning
> var ComponentCount : Integer


---  
 #  EditorViewportHidden : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Hidden from view used for editor.
> ``` lang=cpp, name=Lightning
> var EditorViewportHidden : Boolean


---  
 #  GameSession : [gamesession](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gamesession.md)

 `read-only`

> Get the GameSession that owns us and our Space.
> ``` lang=cpp, name=Lightning
> var GameSession : GameSession


---  
 #  LevelSettings : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> Get the object named 'LevelSettings', a special convenience object where we can put general functionality for our Level.
> ``` lang=cpp, name=Lightning
> var LevelSettings : Cog


---  
 #  Locked : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Not able to be modified or selected in the viewport.
> ``` lang=cpp, name=Lightning
> var Locked : Boolean


---  
 #  MarkedForDestruction : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

 `read-only`

> Has this Cog already been destroyed and is waiting for the frame to end (delayed destruction). This allows us to do custom logic when an object is still not null, but about to be destroyed (e.g. we don't want to render Cogs marked for deletion).
> ``` lang=cpp, name=Lightning
> var MarkedForDestruction : Boolean


---  
 #  Name : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

> Name of the Object.
> ``` lang=cpp, name=Lightning
> var Name : String


---  
 #  ObjectViewHidden : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> If the object needs to not show up in the object view.
> ``` lang=cpp, name=Lightning
> var ObjectViewHidden : Boolean


---  
 #  Parent : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

 `read-only`

> Get the parent of this object in the Hierarchy.
> ``` lang=cpp, name=Lightning
> var Parent : Cog


---  
 #  Persistent : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Object will not be destroyed on level load or change.
> ``` lang=cpp, name=Lightning
> var Persistent : Boolean


---  
 #  RuntimeId : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

 `read-only`

> Gets a unique integer for this object (used primarily for debugging)
> ``` lang=cpp, name=Lightning
> var RuntimeId : Integer


---  
 #  Space : [space](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/space.md)

 `read-only`

> Returns the Space that this object lives in.
> ``` lang=cpp, name=Lightning
> var Space : Space


---  
 #  Transient : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Object will not be saved.
> ``` lang=cpp, name=Lightning
> var Transient : Boolean


---  
 #  Methods


---  
 #  AddComponentByName : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Add a component by name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function AddComponentByName(name : String) : Boolean
> ``` 


---  
 #  AddComponentByType : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Add a component of the given type.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boundtype.md)| |
> ``` lang=cpp, name=Lightning
> function AddComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  AttachTo : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Attach to a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AttachTo(parent : Cog) : Boolean
> ``` 


---  
 #  AttachToPreserveLocal : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Attach to a parent object.
> |Name|Type|Description|
> |---|---|---|
> |parent|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function AttachToPreserveLocal(parent : Cog) : Boolean
> ``` 


---  
 #  ClearArchetype : Void

> Removes our association with the current Archetype.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function ClearArchetype()
> ``` 


---  
 #  Clone : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Clones this cog. The cloned object will be parented to this objects parent (if it exists).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Clone() : Cog
> ``` 


---  
 #  Cog : Void

 `constructor`

> Constructor / destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Cog()
> ``` 


---  
 #  DebugDraw : Void

> Calls DebugDraw on all components in this cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugDraw()
> ``` 


---  
 #  Destroy : Void

> Queues the cog up for delayed destruction (at the end of the frame). If the object is marked as Protected, this will do nothing.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Destroy()
> ``` 


---  
 #  Detach : Void

> Detach from a parent object and compute the new transform so that the objects are relative.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Detach()
> ``` 


---  
 #  DetachPreserveLocal : Void

> Detach from a parent object.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DetachPreserveLocal()
> ``` 


---  
 #  DispatchDown : Void

> Dispatches an event down the tree on all children recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchDown(eventId : String, event : Event)
> ``` 


---  
 #  DispatchEvent : Void

> Dispatches an event on this object.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchEvent(eventId : String, event : Event)
> ``` 


---  
 #  DispatchUp : Void

> Dispatches an event up the tree on each parent recursively (pre-order traversal)
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> |event|[event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Lightning
> function DispatchUp(eventId : String, event : Event)
> ``` 


---  
 #  FindAllChildrenByName : [hierarchynamerange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/hierarchynamerange.md)

> Returns a range of all children with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindAllChildrenByName(name : String) : HierarchyNameRange
> ``` 


---  
 #  FindChildByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Depth first search of all children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindChildByName(name : String) : Cog
> ``` 


---  
 #  FindDirectChildByName : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Checks only direct children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function FindDirectChildByName(name : String) : Cog
> ``` 


---  
 #  FindNearestArchetype : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Same as FindNearestParentArchetype except that it includes this Cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindNearestArchetype() : Cog
> ``` 


---  
 #  FindNextInOrder : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Finds the next Cog in depth first post-order.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindNextInOrder() : Cog
> ``` 


---  
 #  FindNextSibling : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Returns the sibling Cog after this in the parents child list. Returns null if it's the last child. If the Cog doesn't have a parent, it will return the Cog after it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindNextSibling() : Cog
> ``` 


---  
 #  FindPreviousInOrder : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Finds the previous Cog in reverse depth first post-order (the opposite of FindNextInOrder).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindPreviousInOrder() : Cog
> ``` 


---  
 #  FindPreviousSibling : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Returns the sibling Cog before this in the parents child list. Returns null if it's the first child. If the Cog doesn't have a parent, it will return the Cog before it in the Space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindPreviousSibling() : Cog
> ``` 


---  
 #  FindRoot : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Searches up the hierarchy for the root Cog.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindRoot() : Cog
> ``` 


---  
 #  FindRootArchetype : [cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)

> Finds the top most Archetype in the Hierarchy.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function FindRootArchetype() : Cog
> ``` 


---  
 #  GetComponentByIndex : [component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)

> Returns the Component at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)| |
> ``` lang=cpp, name=Lightning
> function GetComponentByIndex(index : Integer) : Component
> ``` 


---  
 #  GetComponentByName : [component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)

> Finds the Components with the given type name.
> |Name|Type|Description|
> |---|---|---|
> |componentTypeName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function GetComponentByName(componentTypeName : String) : Component
> ``` 


---  
 #  GetComponentIndex : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)

> Finds the index of the given Component type. Returns uint max if the Component didn't exist.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boundtype.md)| |
> ``` lang=cpp, name=Lightning
> function GetComponentIndex(componentType : BoundType) : Integer
> ``` 


---  
 #  IsAncestorOf : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not we are an ancestor of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |descendant|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function IsAncestorOf(descendant : Cog) : Boolean
> ``` 


---  
 #  IsDescendant : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not the given cog is a descendant of us.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function IsDescendant(cog : Cog) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not we are a descendant of the given Cog.
> |Name|Type|Description|
> |---|---|---|
> |ancestor|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function IsDescendantOf(ancestor : Cog) : Boolean
> ``` 


---  
 #  IsModifiedFromArchetype : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Returns whether or not we have any local modifications from our Archetype. This does not account for properties with LocalModificationOverride (such as Transform modifications).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function IsModifiedFromArchetype() : Boolean
> ``` 


---  
 #  PlaceAfterSibling : Void

> Moves this Cog after the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function PlaceAfterSibling(sibling : Cog)
> ``` 


---  
 #  PlaceBeforeSibling : Void

> Moves this Cog before the given sibling. Assumes they have the same parent.
> |Name|Type|Description|
> |---|---|---|
> |sibling|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function PlaceBeforeSibling(sibling : Cog)
> ``` 


---  
 #  RemoveComponentByName : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Remove a component by name. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |typeName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveComponentByName(typeName : String) : Boolean
> ``` 


---  
 #  RemoveComponentByType : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md)

> Remove a component by type. Returns true if the component existed.
> |Name|Type|Description|
> |---|---|---|
> |componentType|[boundtype](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boundtype.md)| |
> ``` lang=cpp, name=Lightning
> function RemoveComponentByType(componentType : BoundType) : Boolean
> ``` 


---  
 #  ReplaceChild : Void

> Places the new child at the same place as the old child in the Hierarchy. This detaches but does not destroy the old child.
> |Name|Type|Description|
> |---|---|---|
> |oldChild|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> |newChild|[cog](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Lightning
> function ReplaceChild(oldChild : Cog, newChild : Cog)
> ``` 


---  
 #  SanitizeName : [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)

 `static`

> Cleans an object name of invalid runes.
> |Name|Type|Description|
> |---|---|---|
> |newName|[string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md)| |
> ``` lang=cpp, name=Lightning
> function SanitizeName(newName : String) : String
> ``` 


---  
 #  UploadToArchetype : Void

> Upload this objects data to the archetype and marks this object as not modified. This function does not rebuild all other Cogs with the same Archetype. See ArchetypeRebuilder for more information about how to rebuild Archetypes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UploadToArchetype()
> ``` 


---  
 

 
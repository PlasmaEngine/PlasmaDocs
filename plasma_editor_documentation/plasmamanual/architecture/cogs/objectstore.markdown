
[objectstore](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/objectstore.markdown) saves an object to a persistent local store.  All properties that are normally saved on the object are saved with ObjectStore.  The data is stored on the local computer and will be saved between runs of the game.  Can be used for progress, game saving, or preferences. 

When used with Lightning, make sure you mark the data to be saved with either `[Serialized]` or `[Property]` attributes. 

```lang=csharp
class ObjectStoreTest : LightningComponent
{
    [Property]
    var SomeArchetype : Archetype = null

    function Initialize(init : CogInitializer)
    {
        //just some simple stuff here to cause compilation to work
        var someObject : Cog = null;        
        
        //Restore an object called "Name" and if it does not exist use  SomeArchetype to create it.
        //Also takes the space to create the object in.
        var object = Plasma.ObjectStore.RestoreOrArchetype("Name", "Archetype", this.Space);
        
        //Store the object on local computer
        Plasma.ObjectStore.Store("Name", someObject);
        
        //Restore an object. Null object if not found.
        Plasma.ObjectStore.Restore("Name", this.Space);
    }
}
```
To clear all stored objects on a computer you can use the [ ClearStore ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/command_reference.markdown#clearobjectstore) command.

---

 # Related Materials
 ## Code Reference
- [ ClearStore ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/command_reference.markdown#clearobjectstore) 
 ## Tutorial
- [Loading and Saving Data](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/tutorials/architecture/objectstore.markdown) 

 
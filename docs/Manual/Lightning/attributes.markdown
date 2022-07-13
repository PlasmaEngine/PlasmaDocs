# Attributes

Attributes are part of the Lightning grammar allowing additional information to be associated with other Lightning constructs, i.e. they may be applied to classes, fields, get-sets, and functions. While some attributes are inherent to the Lightning programming language, the program embedding Lightning may create and assign their own meaning to new attributes as appropriate for their scripting needs. This means that some attributes exist in Lightning, the standalone language, while others are available in Lightning due to the extensions made by the Plasma Engine in which it is embedded. 

 # Using Attributes

In Lightning, attributes can be assigned by annotating the affected construct with a capitalized name of the recognized attribute in square brackets above the definition:

<pre><code class="language-csharp" name="Assigning an Attribute to a Function">
[Virtual] // Here we've added the attribute "Virtual" to the function Speak
function Speak() : String
{
  return "...";
}
</code></pre>

 # Existing Attributes

The following are usable in the Plasma Engine:

| Attribute                               | From  | High Concept                                                |
|-----------------------------------------|-------|-------------------------------------------------------------|
| `[Static]`                              | Lightning | Makes construct static                                      |
| `[Virtual]`                             | Lightning | Marks a construct as a polymorphic base                     |
| `[Override]`                            | Lightning | Marks a construct as overriding a base construct            |
| `[Extension(typeid(OtherType))]`        | Lightning | Appends construct to preexisting `OtherType`                |
| `[Display]`                            | Plasma  | Allows construct to appear in Property Grid                 |
| `[Serialize]`                          | Plasma  | Allows construct value to be saved by Plasma                  |
| `[Property]`                            | Plasma  | Combines `[Display]` and `[Serialize]`                    |
| `[Dependency]`                          | Plasma  | Enables Plasma to enforce explicit dependencies               |
| `[RunInEditor]`                         | Plasma  | Allows code to run in the editor                            |
| `[Tool]`                                | Plasma  | Can run in editor and accessible in Tools Window            |
| `[Command]`                             | Plasma  | Can run in editor and accessible in Search Window           |
| `[ComponentInterface]`                  | Plasma  | Defines a class as a generic interface for derived classes  |

 ## [Static]
        
Static can be used on function, fields, and get-sets. These allow you to access fields, get-sets, and functions without first creating an instance of the class in your code. 

<pre><code class="language-csharp" name="Defining a Static Variable and Function">
  class Mathematics
  {
      [Static]
      var PI: Real{ get{return 3.14159292;}}
      [Static]
      function Circumference(radius : Real) : Real
      {
          return Mathematics.PI * radius * radius;
      }
  }
</code></pre>
Given the class above you can use its functionality by calling into the class's namespace:

<pre><code class="language-csharp" name="Using Static Variable and Function">
  var myNewFavoriteNumber = Mathematics.PI + Mathematics.Circumference(2.0);
  Console.WriteLine(My new favorite number is: `myNewFavoriteNumber`");
</code></pre>

will result in 

<pre><code name="ConsoleWindow">
My new favorite number is: 15.708
</code></pre>

NOTE: While these attributes enable polymorphism, they are still in their infancy. Virtual is to be used with the base class field/get-set/function, while Override is for all the derived classes seeking to write over the base class's field/get-set/function. That said, mixing up `[Virtual]` and `[Override]` , or forgetting the use of the `[Override]` may still provide desired results. To promote forward compatibility, we highly encourage the correct, indicated usage.

 ## [Virtual]

Virtual is used to give Base classes the ability to determine some functions as being able to be overridden by its derived classes.

<pre><code class="language-csharp" name="Applying Virtual to a Function">
class Animal
{
  [Virtual]
  function Speak() : String
  {
    return "...";
  }
}
</code></pre>

 ## [Override]
Override is used by a derived class to mark the intentional overriding of a base class's virtual function.

<pre><code class="language-csharp" name="Applying Override to a Function">
class Dog : Animal
{
  [Override]
  function Speak() : String
  {
    return "Woof";
  }
}
</code></pre>

 ## [Extension(typeid(OtherType))]

This allow you to add functionality to a preexisting class from inside another. Currently, you can only extend a class by adding get-sets and functions (i.e. you cannot add fields). If a function is being added to an existing class (`Math`, for example), the [Static] attribute should also be used:

<pre><code class="language-csharp" name="Applying Extension Attribute to a Function">
class MyClass : LightningComponent
{
  [Extension(typeid(Math))][Static]
  function Circumference(radius : Real) : Real
  {
    return Mathematics.PI * radius * radius;
  }
}
</code></pre>

Plasma works with Lightning to offer these additional attributes:

 ## [Display]

Allows you to set a field or get-set via the Property Grid in the editor. Because this doesn't save the settings, it is usually used in conjunction with either `[RunInEditor]` or `[Serialize]` . For example, changing

<pre><code class="language-csharp" name="Variable without Display Attribute">
class MyClass : LightningComponent
{
  var MyVariable : Real;
}
</code></pre>
to

<pre><code class="language-csharp" name="Variable with Display Attribute">
[Editiable]
var MyVariable : Real;
</code></pre>

results in the the variable appearing in the Property Grid in Properties window


 ## [Serialize]

Allows a value to be saved by the Engine. This allows a field and get-sets to be saved with ObjectStore. When used with `[Display]` it allows the values to be saved from the Property Grid so that they may be loaded in an instance of the game. 

 ## [Property]

Property wraps the `[Display]` and `[Serialize]` attributes together into one. As implied by the use of `[Display]` and `[Serialize]`, it works on fields and get-sets. Properties of certain types will result in unique set fields in the Property Grid. For example,

<pre><code class="language-csharp" name="Variables with Property Attribute">
class MyClass
{
  [Property]
  var MyColor : Real4;

  [Property]
  var  MyMaterial : Material;
}
</code></pre>


 ## [Dependency]

Allows the programmer to make a dependency between components explicit. This allows users to determine the interrelatedness without having intimate knowledge of a component's inner workings. The Plasma Engine supports this by requiring dependencies to be added prior to attaching the component, preventing the removal of dependencies while the component is still attached, and safeguarding the order of initialization of components such that the dependencies will always be initialized first. 

The below sample demonstrates the declaration of a dependence upon another component:

<pre><code class="language-csharp" name="Applying the Dependence Attribute on Another Component">
  class SimpleOffset : LightningComponent
  {
      // Declaring that SimpleOffset depends upon Transform component.
      [Dependency]
      var Transform : Transform = null; 
      function Initialize(init : CogInitializer)
      {
          // This declaration also physically adds that variable to our fields: 
          // Since this.Transform contains the component we have a dependency 
          // on, we can access it without going through the Owner. 
          this.Transform.Translation += Real3(0,5,0);
      }
  }
</code></pre>

The `[Dependency]` attribute may also be used on get-sets.

NOTE: **Did you know?** When working in the editor, the space the objects operate in is paused. This means that the `LogicUpdate` event will never fire, and that Actions on objects never get updated! In order to receive continuous events, the object should connect to `UpdateFrame` instead.


 ## [RunInEditor]

When placed on a class derived from LightningComponent, it changes proxy objects into live objects upon being attached in the editor. This means that the object will run its code in the editor. When *any* scripting file is saved in the editor, all live objects (i.e. those with the RunInEditor component attached) will, by default, have their object destroyed, recreated, and its data reinitialized. 

IMPORTANT: Any code you choose to run via `[RunInEditor]` can result in editor instability. For instance, if you choose to loop through and destroy all the objects and save your game you may lose your ability to recover the lost objects, and have to recreate them by hand. Undo and Redo operations for RunInEditor components must be handled by the programmer!  

 ## [Tool]

Allows for a tool to be hooked into the Tools Window such that it shows up in the drop down menu, and can be used in the editor. When creating a new custom tool, a good starting point is generating the LightningScript with the Tool template chosen in the Add Window.

 ## [Command]

Allows for a class to be hooked into the command system such that it shows up, and can be ran, from Plasma's Search Window. The following Paste provides a template for a custom Command that creates an object based on an archetype, allowing the user to make their own "Create" commands similar to `CreateCube` and `CreateSphere`:

```
[Command(autoRegister:true)]
class CreateArchetype : LightningComponent
{
  // The archetype from which to create an object
  var ArchetypeToCreate : Archetype = Archetype.MyObject;
  
  // The position at which to create the object
  var Position : Real3 = Real3(0, 1, 0);
  
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.Owner, Events.CommandExecute, this.OnCommandExecute);
  }

  function OnCommandExecute(event : CommandEvent)
  {
    var selection = Plasma.Editor.Selection;
    selection.SelectOnly(this);
    selection.FinalSelectionChanged();
    
    this.CreateObject();
  }
  
  function CreateObject()
  {
    // Create the object in Editor space
    var editorSpace = Plasma.Editor.EditSpace;
    editorSpace.CreateAtPosition(this.ArchetypeToCreate, this.Position);
  }
}

```


 ## [ComponentInterface]
The ComponentInterface attribute allows the user to define a class as a generic interface for its derived types. One common example of this is [collider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/collider.markdown), which acts as a component interface for all collider types, such as [boxcollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/boxcollider.markdown), [capsulecollider](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/capsulecollider.markdown), and more. Defining an interface using this attribute allows the user to access the members of a derived class using the component name of the base class.

<pre><code class="language-csharp" name="Component Interface Access Example">
var collisionGroup = this.Owner.BoxCollider.CollisionGroup;
var collisionGroupAccessedByInterface = this.Owner.Collider.CollisionGroup;

if(collisionGroup == collisionGroupAccessedByInterface)
  Console.WriteLine("These variables reference the same component");
</code></pre>

Using a component interface does not mean that the property and methods of a derived class need to be exactly the same as the base class. What would be the point? Using the [ Virtual](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/sandbox/arend_danielek/attributes.markdown#virtual) and [ Override ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/sandbox/arend_danielek/attributes.markdown#override) attributes, we can modify the interface of derived classes.

<pre><code class="language-csharp" name="Component Interface Example">
[ComponentInterface]
class AnimationDebugNode : LightningComponent
{
  [Virtual]
  var Node : AnimationNode;
  
  function Initialize(init : CogInitializer)
  {
    
  }
}

class SelectiveDebugNode : AnimationDebugNode
{
  [Override]
  var Node : SelectiveNode;
}

class DirectBlendDebugNode : AnimationDebugNode
{
  [Override]
  var Node : DirectBlend;
}

class CrossBlendDebugNode : AnimationDebugNode
{
  [Override]
  var Node : CrossBlend;
}
</code></pre>

 # Parameters in Attributes

Attributes can also take parameters; below is the template generated for creating a new Command by Plasma:

<pre><code class="language-csharp">
[Command(autoRegister:true)] // This template file sets a parameter, autoRegister, to true.
class MyNewCommand : LightningComponent
{
  function Initialize(init : CogInitializer)
  {
      Plasma.Connect(this.Owner, Events.CommandExecute, this.OnCommandExecute);
  }

  function OnCommandExecute(event : CommandEvent)
  {
    Console.WriteLine("MyNewCommand Command Executed");
  }
}
</code></pre>

At this time, only Extension, Tool, and Command attributes take parameters. 

 - Extension requires the type you are using to extend the attribute, as a parameter. 

 - Tool and Command have the optional parameter to automatically register the component with the engine. 

To manually register, you would add these components to an archetype and then add the Tool or Command editor tag via the Library Window, respectively. Registering manually gives you access to the archetype, making it possible to leverage component-based design in the construction of new Tools and Commands.

 # Related Materials
 ## Manual
- [inheritance](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/Lightning/inheritance.markdown)
- [variables_and_data_types](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/Lightning/variables_and_data_types.markdown)
- [wysiwyg](https://plasmaengine.github.io/PlasmaDocs/Manual/plasmamanual/scripting/wysiwyg.markdown) 

 
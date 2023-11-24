
 # Variables
Variables are used to store data, and are declared using the `var` keyword.  Each variable in lightning has a name, a type, and a value which must be declared within a class using the following syntax.

`var Name : Type = value;`

<pre><code class="language-csharp">
var Greeting : String = "Hello";
var Sum : Real = 1 + 2;
var Up : Real3 = Real3(0,1,0);
</code></pre>

`var` is the keyword used to indicate that the statement on this line declares a variable. `Greeting` is the **name** of the first variable, an identifier used to reference the [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown) type value `"Hello"`. 

Both `Greeting` and `Sum` follow the following format: `var` `Name` `:` `Type` `=` `"Value"``;`.

| Token | Description |
| `var` | Keyword used to indicate the statement declares a variable. |
| `Name` | Name of the variable. |
| `:` | Delimiter indicating the next identifier in the line is the type of the variable being declared. |
| `Type` | Type of the variable being declared. |
| `=` | Assignment operator used to initialize the variable to a value. |
| `"Value"` | Value for the variable to be initialized to. |
| `;` | Delimiter indicating the end of the statement. |

NOTE: Identifier names must be alphanumeric and may include underscores. They cannot start with a number, and no other symbols are allowed. Remember to choose identifier names that don't clash with the [Keywords](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.markdown) or [Lightning Base Types](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types.markdown).

Depending on the context, or [Scope](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.markdown#scope), the required syntax for instantiating and initializing a variable can vary.  The codeblock above will only compile if placed at the scope of a class or struct.

(NOTE)**Literal Types**: Literal values are values explicitly defined by the user in script.  `1 + 2` is an example of two literal values that evaluate to the non-literal value `3`.  Below is a table of more literal values and their associated [lightning_base_types](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types.markdown).

 | Literal Value(s) | Type |
 | -- | -- |
 | `1`, `2`, etc. | Integer |
 | `1d`, `2d`, etc. | DoubleInteger |
 | `1.0`, `2.0`, etc. | Real |
 | `1.0d`, `1.0d`, etc. | DoubleReal |
 | `true`/`false` | Boolean |
 | `"Hello"`, `"Goodbye"`, etc. | String |
 | `null` | Null |

 # Scope
A scope is a region in which certain elements of the language, such as variables and functions, are defined.  Any scope can contain multiple nested scopes.  A real-life example of scope could be a building and the rooms inside it.  Whatever is *in* the scope of a room is also *in*, but not *at*, the scope of the building, because the room's scope exists inside the scope of the building. In Lightning, the three most common levels of scope are global, object, and block.

 ## Global Scope
Everything in script exists *in* the **global scope**; however, not everything is created *at* the **global scope**. Libraries such as `Plasma` and `Math` exist //at// the **global scope** and are therefore accessible from any scope in script.  The [plasma](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown) and [Math](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/math.markdown) libraries are objects defined at the global scope. [Classes and Structs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.markdown) are the only Lightning constructs that can be defined //at* the **global scope**.

<pre><code class="language-csharp">
var R1 : Real; //Error, can not declare variables at the global scope

class MyClass : LightningComponent //We can declare definitions of objects such as classes at the global scope
{
}
</code></pre>

Notice in this example that the attempted instantiation of a variable at the **global scope** will throw an exception.

 ## Object Scope
[Classes and Structs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.markdown) define their own scope and are one of the few constructs that exist *at// the **Global Scope**. Variables defined //at* the **object scope** are called **member** variables and will exist as long as the object exists.

<pre><code class="language-csharp">
class MyClass
{
  var Pi : Real = Math.Pi; //compiles
  var Theta : Real; // compiles
  var A = 4.0; //compiles
  var B = -5.0; //does not compile
  var C = PerspectiveMode.Orthographic; //does not compile
}
</code></pre>
Notice in the example above that `Math` *in// the **global scope** is accessed //from* the **class scope** while initializing `MyClass.Pi`.

 ### Implicit Initialization
Notice above that `MyClass.Theta` is not given an **explicit** initial value. This means that **implicit** initialization will take place, assigning `Theta` an initial value of the default type value of the type [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown), which in this case is `0`. Implicit initialization of a variable is only possible when defining a **member** variable. The final restriction for member variables is that they must begin with an upper case letter.

 ### Inferred Typing
In the code block above `MyClass.A` is not given an explcit type. In this situation the type [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) is **inferred** from the the type of its initialization value `4.0`. Only literal, type casted, or manually constructed values may be use for inferred typing when initializing a member variable. Statements such as `var B = -5.0;` will not compile because they contain an expression.

NOTE: You can not use implicit initialization and inferred typing on the same variable.

 ## Block Scope
[functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown), [conditionals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/conditionals.markdown), and [loops](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.markdown) must have their scopes defined within an **object scope**. Variables defined within a **block scope** only exist until the scope is finished being executed. Variables defined within a block scope are called **local variables**.

NOTE: Local variables can be implicitly initialized and have their types inferred just as member variables can.

 ### The Scope Operator
In addition to to logical constructs defining scope, Lightning allows the user to define arbitrary scopes using the [scope](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.markdown) keyword.
<pre><code class="language-csharp">
class MyClass
{
  var M1 : Real = 1.0;
  function MyFunction()
  {
    var r1 = this.M1;
    scope
    {
      var r2 = r1;
    }
    var r3 = r1;
    r3 = r2; //ERROR
  }
}
</code></pre>

In the above example begins with `var r1 = this.M1;` and then demonstrates the use of the {icon university}[[plasma_engine_documentation/plasma_editor_documentation/plasmama
nual/Lightning/keywords/|scope]] keyword.

Inside the inner block scope is the line `var r2 = r1;`. Because `r1` is declared in an outer scope it can be used to initialize `r2`.

The line `var r3 = r1;` follows the closing `}` of the inner block scope. Because `r1` was declared at the same scope as `r3`, it can be used as `r3`'s initialization value. However, the next line, `r3 = r2;`, will result in an error. `r2` was declared in the inner block scope. When that scope closes, `r2` is destroyed. As a result, `r2` is no longer a valid variable, and so it cannot be used to initialize `r3`.

(NOTE)**Data Lifetimes**: It should be noted that when most variables go out of the scope they are declared in they stop existing. This is true for value types such as [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) and [Structs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.markdown). However, if a reference type such as a constructed [Class](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.markdown) instance still has a valid reference being held outside of the instantiation scope it will remain alive in memory.

 # Caching Variables
Caching accessed data into locally scoped variables is a common practice that can improve the efficiency, readability, and flexibility of code. Often users may find themselves needing a value that will be used multiple times throughout the scope it is calculated/accessed in.

<pre><code class="language-csharp">
class Intercept : LightningComponent
{
  [Dependency] var RigidBody : RigidBody;
  
  [Property]
  var PlayerCogPath : CogPath = CogPath();
  
  [Property]
  var Velocity : Real = 5.0;
  
  [Property]
  var MinDistance : Real = 5.0;
  
  [Property]
  var PredictionTime : Real = 1.0;
  
  function Initialize(init : CogInitializer)
  {
    this.Owner.RigidBody.DynamicState = RigidBodyDynamicState.Kinematic;
    Plasma.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var playerCog = this.PlayerCogPath.Cog;
    var playerPos = playerCog.Transform.Translation;
    var myPos = this.Owner.Transform.Translation;
    var distance = Math.Distance(myPos, playerPos);
    
    if(distance <= this.MinDistance)
    {
      var playerVelocity = playerCog.RigidBody.Velocity;
      var predictedPos = playerPos + (playerVelocity * this.PredictionTime);
      var myMoveDir = Math.Normalize(predictedPos - myPos);
      var newPos = myPos + (myMoveDir * this.Velocity * event.Dt);
      this.Owner.Transform.Translation = newPos;
    }
  }
}
</code></pre>
In the above example `playerCog`, `playerPos`, and `myPos` are all examples of caching accessed values to local variables. These pieces of data are needed multiple times in calculations made later in the `OnLogicUpdate` function. By caching these values, not only does writing and reading the calculations become easier, it reduces the number of member data accesses that are necessary via the `.` operator.

<pre><code class="language-csharp">e
function OnLogicUpdate(event : UpdateEvent)
{
  if(Math.Distance(this.Owner.Transform.Translation, this.PlayerCogPath.Cog.Transform.Translation) <= this.MinDistance)
  {
    this.Owner.Transform.Translation = this.Owner.Transform.Translation + (Math.Normalize(this.PlayerCogPath.Cog.Transform.Translation + (this.PlayerCogPath.Cog.RigidBody.Velocity * this.PredictionTime) - this.Owner.Transform.Translation) * this.Velocity * event.Dt);
  }
}
</code></pre>
This example implements the exact same behavior as the previous `OnLogicUdpate` function, but does not cache any variables locally. As can be seen the line count has been reduced, but these few lines are much harder to interpret and contain many duplicate member access operations. While this may seems like a small issue, it is one that may add up rather quickly over time.

 # Related Materials
 ## Manual
- [Classes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.markdown)
- [functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown)
- [Keywords](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.markdown)
- [Scope](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.markdown)
- [Conditionals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/conditionals.markdown)
- [Loops](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.markdown)

 ## Code Reference
- [lightning_base_types](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types.markdown)
- [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)
- [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.markdown)
- [Plasma](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/plasma.markdown)
- [Math](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/math.markdown) 

 
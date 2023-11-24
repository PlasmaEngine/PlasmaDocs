# Enums
An enum, or enumerated type, is a set custom identifiers that are enumerated. An enumerated type may be defined with the **enum** keyword:

<pre><code class="language-csharp">
enum ControllerButtons {Start, Select, Up=0, Down, Left, Right, A=0, B=1} // no semicolon
</code></pre>

The names line up with incrementing [Integers](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown) where the default starting value is 0. The values can be manually set in which case the following values will increment off of that manually defined value. Note that to access these Integer values, the enum must be [casted](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/casting.markdown) to an Integer:
<pre><code class="language-csharp">
Console.WriteLine("ControllerButtons.Start  = `ControllerButtons.Start  as Integer`  " );
Console.WriteLine("ControllerButtons.Select = `ControllerButtons.Select as Integer`  " );
Console.WriteLine("ControllerButtons.Up     = `ControllerButtons.Up     as Integer`  " );
Console.WriteLine("ControllerButtons.Down   = `ControllerButtons.Down   as Integer`  " );
Console.WriteLine("ControllerButtons.Left   = `ControllerButtons.Left   as Integer`  " );
Console.WriteLine("ControllerButtons.Right  = `ControllerButtons.Right  as Integer`  " );
Console.WriteLine("ControllerButtons.A      = `ControllerButtons.A      as Integer`  " );
Console.WriteLine("ControllerButtons.B      = `ControllerButtons.B      as Integer`  " );
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
ControllerButtons.Start  = 0  
ControllerButtons.Select = 1  
ControllerButtons.Up     = 0  
ControllerButtons.Down   = 1  
ControllerButtons.Left   = 2  
ControllerButtons.Right  = 3  
ControllerButtons.A      = 0  
ControllerButtons.B      = 1  
</code></pre>

 # Enum Rules

There a number of rules that must be followed when defining enums. If these rules are not followed, an error will be thrown, as can be seen in the examples below.

 ## Type Name and Value Capitalization

Identifiers for the enum type name and the enumerated values must be capitalized.

<pre><code class="language-csharp">
// This will not compile. 
enum Directions {up, down, left, right}
</code></pre>

<pre><code class="language-csharp">
Enum declaration 'Directions' does not have a closing '}'. We found 'LowerIdentifier' but we expected to find '}'.
</code></pre>

<pre><code class="language-csharp">
// This won't compile either.
enum directions {Up, Down, Left, Right}
</code></pre>

<pre><code class="language-csharp">
Enum declaration is missing a name. Upper-camel case names are required here (use 'Directions'
instead of 'directions').    
</code></pre>


 ## Unique Identifiers

Identifiers for the enumerated values must be unique.

<pre><code class="language-csharp">
// This will not compile.
enum Directions {Up, Down, Up, Down}
</code></pre>

<pre><code class="language-csharp">
A value of the same name 'Up' has already been declared in the enum 'Directions'. Names must 
only be used once.
</code></pre>

 ## Definition Scope

Enums cannot be defined inside classes, structs, or other enums.

<pre><code class="language-csharp">
// Classes cannot contain enums.
class EnumWrapper
{
  // This won't compile.
  enum ControllerButtons {Start, Select, Up=0, Down, Left, Right, A=0, B=1}
}
</code></pre>

<pre><code class="language-csharp">
Class declaration 'EnumWrapper' does not have a closing '}'. We found 'enum' but we expected to find '}'.
</code></pre>

 # Enums and Integers

As in other languages, Integers make up the backbone of how enums work, and thus they work together in many situations.

 ## Casting

Because of this, Lightning will implicitly cast from an enum to an Integer when necessary:

Given this:

<pre><code class="language-csharp">
enum ControllerButtons {Start, Select, Up=0, Down, Left, Right, A=0, B=1}

class Controller
{
  [Static]
  // This function accepts an enum type.
  function AcceptsEnum(param: ControllerButtons)
  {
    Console.WriteLine(" turned into `param`!");
  }
  
  [Static]
  // This function accepts an integer type.
  function AcceptsInt(param: Integer)
  {
    Console.WriteLine(" turned into `param`!");
  }
}
</code></pre>

We can test the calls to these [functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown) to see the interplay of casting:

<pre><code class="language-csharp">
var paramInt = 3;
var paramEnum = ControllerButtons.Right;

// This works, as you'd expect
Console.Write(paramEnum);
Controller.AcceptsEnum(paramEnum);

// But if you want to accept an Integer in an enum's place you MUST cast. 
Console.Write(paramInt);
Controller.AcceptsEnum(paramInt as ControllerButtons);
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
Right turned into Right!
3 turned into Right!    
</code></pre>

<pre><code class="language-csharp">
// Attempting to pass an Integer without casting to an enum 
// will cause a compiler error
Console.Write(paramInt);
Controller.AcceptsEnum(paramInt);
</code></pre>

<pre><code class="language-csharp">
The function 'AcceptsEnum' exists, but could not be resolved since the types of the arguments 
used did not match. The arguments you gave were: 

  AcceptsEnum(Integer)

The possible choices were: 

  AcceptsEnum(param : ControllerButtons)
</code></pre>

<pre><code class="language-csharp">
// This also works as you'd expect. 
Console.Write(paramInt);
Controller.AcceptsInt(paramInt);

// The enum type parameter is implicitly casted to an Integer and is then passed to the function. 
Console.Write(paramEnum);
Controller.AcceptsInt(paramEnum);
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
3 turned into 3!
Right turned into 3!
</code></pre>

 ## Enum-Integer Operations

Enums can perform all operations as if they were Integers. For instance, you can perform all of the normal Integer math operations as implicit conversion will happen as necessary:
<pre><code class="language-csharp">
// Here you can see use of the +, -, *, /, (), ^ and % Integer operators.
var math = (ControllerButtons.Start + ControllerButtons.Right) ^ ControllerButtons.Left % 
           ControllerButtons.Right - ControllerButtons.Right * ControllerButtons.Select;
           
// When the math evaluates to an unaliased number, the variable, although still of the enum type, 
// prints out its integer value.
Console.WriteLine(math); 
Console.WriteLine(typeid(math).Name);
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
-3
ControllerButtons
</code></pre>
Notice that the typeid is not an Integer but `ControllerButtons`. An Integer value was printed because there was no alias in the enum that maps to `-3`.


Because the type is still that of the enum, it can be passed to the `Controller.AcceptsEnum()` function without issue.  

When an operation includes both an enum and an Integer the result is always promoted to the enum type. To get an Integer either 

- Declare the variable you are storing the result in as an Integer: `var result : Integer`
- Cast it: `result as Integer`

 ## Caveat

Although enums cast to Integers, they **will not** cast to Integers to perform cross-enum operations.

<pre><code class="language-csharp">
// This won't compile.
Console.WriteLine(ControllerButtons.Down + Directions.Down);
</code></pre>

<pre><code class="language-csharp">
The binary '+' operator 'Positive / Add' is not valid with 'ControllerButtons' and 'Directions'.
</code></pre>

 # Related Materials
 ## Manual
- [casting](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/casting.markdown)
- [functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown)

 ## Code Reference
- [enum_reference](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown)
- [integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown) 

 
# Reflection
Reflection describes an objects ability to "reflect" on itself, generally this means to understand it's type and relationships to other types. Although Lightning does not boast a robust reflection library it does have a basic typeid for by-value types and [property_delegates](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/property_delegates.md):

 # typeid
<pre><code class="language-csharp">
  var i = 0;
  var di = 0d;
  var real = 0.0;
  var double = 0.0d;
  var word = "";
  var refType = null;
  var boolTrue = true;
  var boolFalse = false;
  var prop = new Property[Real]();        
  
  Console.Write("integer, 0 is of type: ");
  Console.WriteLine(typeid(i).Name);               // integer, 0 is of type: Integer
  Console.Write("doubleinteger, 0d is of type: ");
  Console.WriteLine(typeid(di).Name);              // doubleinteger, 0d is of type: DoubleInteger
  Console.Write("real, 0.0 is of type: ");
  Console.WriteLine(typeid(real).Name);            // real, 0.0 is of type: Real
  Console.Write("doublereal, 0.0d is of type: ");
  Console.WriteLine(typeid(double).Name);          // doublereal, 0.0d is of type: DoubleReal
  Console.Write("string, \"\" is of type: ");
  Console.WriteLine(typeid(word).Name);            // string, "" is of type: String
  Console.Write("null, null is of type: ");
  Console.WriteLine(typeid(refType).Name);         // refTypeHandle, null is of type: Null
  Console.Write("boolean, true is of type: ");
  Console.WriteLine(typeid(boolTrue).Name);        // boolean, true is of type: Boolean
  Console.Write("boolean, false is of type: ");
  Console.WriteLine(typeid(boolFalse).Name);       // boolean, false is of type: Boolean   
  Console.Write("Real property delegate is of type: "); 
  Console.WriteLine(typeid(prop).Name);            // Real property delegate is of type: Property[Real]
</code></pre>

<pre><code class="language-csharp">
  ---------------- Begin Game ---------------
  integer, 0 is of type: Integer
  doubleinteger, 0d is of type: DoubleInteger
  real, 0.0 is of type: Real
  doublereal, 0.0d is of type: DoubleReal
  string, "" is of type: String
  null, null is of type: Null
  boolean, true is of type: Boolean
  boolean, false is of type: Boolean
  Real property delegate is of type: Property[Real]
</code></pre>
--------------------
 # String Interpolation

Those types that are [memory_management](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/memory_management.md) or [delegates](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/delegates.md) types can be inspected with [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/lightning_base_types/string.md) Interpolation:

<pre><code class="language-csharp">
class Utility
{
  constructor()
  {
  }
  [Static]
  function HelloWorld()
  {
    Console.WriteLine("Hello World");
  }
  
  function Add(a: Integer, b: Integer): Integer
  {
    return a+b;
  }
}

class Driver 
{
  function TypeidForRefAndDelegates()
  {
    var del = Utility.HelloWorld;
    var temp = new Utility();
    var del2 = temp.Add;
    var vectorRef = new Real3(0.0, 1.0, 2.0);

    Console.Write("delegate(), Utility.HelloWorld can be string interpolated to read: "); 
    Console.WriteLine("`del`");
    
    Console.Write("delegate(a:Integer, b:Integer):Integer, Utility.Add");
    Console.Write(" can be string interpolated to read: ");
    Console.WriteLine("`del2`");

    
    Console.Write("ref Real3, (0.0, 1.0, 2.0) is of type: ");
    Console.WriteLine("`vectorRef`");
  }
}
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
delegate(), Utility.HelloWorld can be string interpolated to read: Utility.HelloWorld()
delegate(a:Integer, b:Integer):Integer, Utility.Add can be string interpolated to read: 
Utility.Add(a : Integer, b : Integer) : Integer
ref Real3, (0.0, 1.0, 2.0) is of type: ref Real3
</code></pre>
--------------

 # Console.DumpValue

Useful in understanding the current state of a Lightning object, Console.DumpValue prints out the names of the variables and their type, if a [class](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md), or their value if a basic, built-in data type.

<pre><code class="language-csharp">
class TopLevel
{
  var MyVariable: MidLevel = null;
  constructor()
  {
  }
}

class MidLevel
{
  var MyVariable: BottomLevel = BottomLevel(false);
  constructor()
  {
  }
}

struct BottomLevel
{
  var IsBottom: Boolean = true;
  var UpAxis: Real3 = Real3(0.0, 1.0, 0.0);
  constructor(param: Boolean)
  {
    this.IsBottom = param;
  }
}
    
class ReflectionDriver
{
  [Static]
  function Dumping()
  {
    var top = TopLevel();
    var mid = MidLevel();
    var bot = BottomLevel(true);
    
    Console.DumpValue(top);
    Console.DumpValue(mid, 8); // The second parameter indicates the depth of recursion cut-off
    Console.DumpValue(bot);
    
  }
}
</code></pre>

<pre><code class="language-csharp">
---------------- Begin Game ---------------
TopLevel
  MyVariable: (null) MidLevel
MidLevel
  MyVariable: BottomLevel
    IsBottom: False
    UpAxis: (0, 1, 0)
      X: 0
      Y: 1
      Z: 0
BottomLevel
  IsBottom: True
  UpAxis: (0, 1, 0)
</code></pre>

*Notice how the MidLevel dumps more information than the BottomLevel with comparable information, due to the second parameter.*

 # Related Materials
 ## Manual

- [property_delegates](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/property_delegates.md)
- [memory_management](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/memory_management.md)
- [delegates](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/delegates.md)
- [string](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/lightning_base_types/string.md)
- [classes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md)
 

 
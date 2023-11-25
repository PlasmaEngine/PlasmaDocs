# Inheritance
Inheritance allows a *child [class](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md) to automatically receive all of the data and functionality defined within the base* class.

<pre><code class="language-csharp">
class Feline
{
  constructor() { }
}
</code></pre>

<pre><code class="language-csharp">
// A colon designates an identifier for a base class follows.
class Lion : Feline
{
  // a constructor is not necessary when one is inherited from the base class.  
}
</code></pre>
<pre><code class="language-csharp">
var cat = new Feline();
var simba = new Lion(); // Instantiated from the inherited constructor
</code></pre>

In the above example the variable `simba` can be instantiated as a `Lion` using the constructor from `Feline`.

 # The **base** Keyword
The **base** [keyword](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.md) is for use when defining an inherited class; it allows you to call the constructor of the base class being inherited from before running an explicitly defined constructor.

<pre><code class="language-csharp">
class Animal
{
  var Legs : Integer = 4;
  
  constructor() { }
  constructor(legs : Integer)
  {
      this.Legs = legs;
  }

  function ToString() : String
  {
    var builder = new StringBuilder();
    builder.Write("Legs: ");
    builder.Write(this.Legs);
    return builder.ToString();
  }
}
</code></pre>
The class animal defines a **non-default** constructor which takes a number of legs for the animal as a parameter.

<pre><code class="language-csharp">
class Human : Animal
{
  constructor() : base(2) { }
}
</code></pre>
The class `Human` which inherits from `Animal` can use `Animal`'s constructor by using the `base` keyword. In this situation either the default or non-default constructor from `Animal` could be called using based. Which constructor is called is determined by the parameters passed to the `()` after the`base` keyword. Because `2` is passed to the `base` keyword the **non-default** constructor of `Animal` is called before any implementation within the defined **default** constructor of `Human`.

<pre><code class="language-csharp">
var animal : Animal = new Animal();
Console.WriteLine(animal.ToString()); // Legs: 4

var jerry = new Human();
Console.WriteLine(jerry.ToString());  // Legs: 2
</code></pre>
In this runtime example both `Animal` and `Human` are instantiated using their default constructor.

<pre><code class="language-csharp">
---------------- Begin Game ---------------
Legs: 4
Legs: 2
</code></pre>
As can be seen in the console output the `Human` **default** constructor calls the **non-default** constructor of `Animal` and passes it `2`.

 # Classes & Structs
Although Lightning currently does not throw an error, erratic and unexpected behavior will result from having a class inherit from a struct and vice versa. **i.e.**

<pre><code class="language-csharp">
// Mismatching the struct/class between parent and child
struct MyBaseStruct
{
  constructor()
  {
  }
}
class MyClass : MyBaseStruct
{
  constructor() : base()
  {
  }
}
</code></pre>
<pre><code class="language-csharp">
// Leads to issues such as the inability to cast to the base class type. 
var incompatible: MyClass = new MyClass();
Console.WriteLine(typeid(incompatible).Name);                 // MyClass
Console.WriteLine(typeid(incompatible as MyBaseStruct).Name); // This won't compile.
</code></pre>

 # The Virtual Keyword

Virtual is used to give Base classes the ability to determine some functions as being able to be *overridden* by its derived classes. The new `Speak` function defined in `Animal` will serve as an example:

<pre><code class="language-csharp">
class Animal
{
  var Legs:Integer = 4;

  constructor() { }
  
  constructor(legs : Integer)
  {
    this.Legs = legs;
  }
  
  function ToString() : String
  {
    var builder = new StringBuilder();
    builder.Write("Legs: ");
    builder.Write(this.Legs);
    return builder.ToString();
  }
  
  [Virtual]
  function Speak() : String
  {
    return "...";
  }
}
</code></pre>

By default, animals don't say anything, so a string that says `...` is returned. It is known that there are animals that do speak, so the `[Virtual]` attribute is added to the function to let other developers know that if a class is is **derived** from `Animal`, the functionality of `Speak` may be overridden.


<pre><code class="language-csharp">
class Human : Animal
{
  constructor() : base(2) { }
  
  [Override]
  function Speak() : String
  {
    return "Hello";
  }
}
</code></pre>
Humans do speak, so changeing the funcitonality of `Human.Speak` to say something other than `...` makes perfect sense. The `[Override]` attribute applied to `Speak` marks this implementation of the `Speak` function to replace `Animal.Speak` which is marked as `[Virtual]`.

This can also be extended to other classes like a Cat:

<pre><code class="language-csharp">
class Cat : Animal
{
  // Cats have 4 legs, so let's update the constructor
  constructor() : base(4) { }
  
  [Override]
  function Speak() : String
  {
    return "Meow";
  }
}
</code></pre>

Now, this is great in the fact that we can now do something like the following:

<pre><code class="language-csharp">
var animal = Animal();
Console.WriteLine(animal.Speak());

var human = Human();
Console.WriteLine(human.Speak());

var cat = Cat();
Console.WriteLine(cat.Speak());
</code></pre>

<pre><code class="language-csharp">
...
Hello
Meow
</code></pre>

The real magic of inheritance comes in the idea that a class of a **derived** class can be stored in a variable that matches the type of the **base** class.

<pre><code class="language-csharp">
var humanIsAnAnimal : Animal = Human();
Console.WriteLine(humanIsAnAnimal.Speak());
</code></pre>

Even though the variable is of type Animal, the Human version of the function is called:

<pre><code class="language-csharp">
Hello
</code></pre>

This is because whenever a virtual method is called, the run-time type of the object is checked for an **overriding member**. The overriding member in the most derived class will then be called, which might be the original function if the derived class(es) have not overridden it.

This can be quite useful with an array of Animals.

<pre><code class="language-csharp">
var a : Animal = Animal();
var b : Human = Human();
var c : Animal = Human();
var d : Cat = Cat();

var array : Array[Animal] = Array[Animal](){a,b,c,d};

foreach (var animal in array)
{
  Console.WriteLine(animal.Speak());
}
</code></pre>


<pre><code class="language-csharp">
...
Hello
Hello
Meow
</code></pre>

 # Calling Parent Functions

It's also possible to call the parent version of a function from a child class. In order to do this, the object must be cast to the base type and then use the non-virtual operator (~>) to call the base version:

<pre><code class="language-csharp">
var d : Cat = Cat();
(d as Animal)~>Speak();
</code></pre>
<pre><code class="language-csharp">
...
</code></pre>

 # Related Materials
 ## Manual
- [attributes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.md) 

 
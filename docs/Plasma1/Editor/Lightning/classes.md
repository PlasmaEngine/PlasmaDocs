# Classes

Classes and structs define the type of certain objects in Lightning, and the `class` keyword can create user-defined data types.  The [Variables](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.md) and [Functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.md) defined in a class or struct are all stored and referenced from instantiations.  In contrast with how Structs handle [Memory Management](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/memory_management.md), classes are copied `by-reference`.

# Class Contents
Classes in Lightning must be defined in [global scope](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.md#global-scope).  The format for classes and structs are as shown below:

<pre><code class="language-csharp" name="Simple Classes">
struct SimpleStruct {}
class SimpleClass {}
</code></pre>

Any members that belong to `SimpleStruct` or `SimpleClass` will be defined within their curly braces.

## Struct Members in Classes
Because structs are copied `by-value`, structs cannot have class members.  As shown in the code snippet below, any other permutation of containment is valid.

<pre><code class="language-csharp" name="Classes and Structs in Classes and Structs">
struct StructInStruct { var MyStruct : SimpleStruct; }
struct ClassInStruct { var MyClass : SimpleClass; } // ERROR
class StructInClass { var MyStruct : SimpleStruct; }
class ClassInClass { var MyClass : SimpleClass; }
</code></pre>

The class `MyClass` is a member of `ClassInStruct`, which is a struct.  Having a class in a struct will cause Lightning to throw a compile-time exception.

## Static vs Non-Static Members
Variables and functions inside a class or struct are known as members. Most member variables must be accessed through instantiations of the object.  The one exception are member variables with the [Static](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.md#static) [Attribute](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.md).

<pre><code class="language-csharp" name="Static Members">
class MyClass
{
  // standard variable instantiation and initialization
  var MyReal : Real = 0;
  
  // static variable
  [Static]
  var MyStaticBoolean : Boolean = false;
  
  // static function
  [Static]
  function MyStaticFunction() {}
}
</code></pre>

Accessing static members can be done with `MyVariableClass.MyStaticReal` or `MyVariableClass.MyStaticFunction`, while `MyVariableClass().MyReal` is a way of accessing a non-static member.

 ## Member Variable Declaration
Member variables define the data in a class.  The rules for defining member variables differ from how local variables are defined.

<pre><code class="language-csharp" name="Member Variables">
class MyClass
{
  // variable instantiation only is allowed
  var MyDoubleReal : DoubleReal;
  
  // ERROR: type deduction not allowed on member variables
  var MyBoolean = false;
}
</code></pre>

Notice how `MyDoubleReal` isn't initialized.  At the class scope, uninitialized member variables will be set to the default values of their types. Also note that member variables must be explicitly typed.  `MyBoolean` is set to `false`, but Lightning will still throw a compiler error if the type is omitted.

## Member Functions
Member functions hold executable code, can take input parameters, and can return data.  Member functions without the `[Static]` attribute  also have access to the instantiated object that invoked them.

<pre><code class="language-csharp" name="Member Functions">
class MyClass
{
  var MyReal : Real = 1.2;
  
  function MyFunc()
  {
    var localReal = this.MyReal;
  }
  
  [Static]
  function MyFunc()
  {
    var localReal = this.MyReal; // ERROR
  }
}
</code></pre>

Notice how `MyReal`, a member variable of `MyClass`, is accessed in `MyFunc` using the `this` keyword.  `this` refers to the instantiated object.  If the function is static, then `this` cannot be used as there is no instantiation of `MyClass`.  Also notice how there are two versions of `MyFunc`, one static and one not.  This is valid because static members must always be accessed through the class with the format `<class>.<function>`.

## Constructors and Destructors
Structs/Classes can have constructor and destructors, which are special functions with no return type.  Constructors are called when an object is instantiated, and the destructor is called when the object is deleted.

<pre><code class="language-csharp" name="Default Constructor">
class ExplicitDefault
{
  constructor() {}
}

class ImplicitDefault {}

class Driver
{
  function MyFunction()
  {
    ExplicitDefault(); // call default constructor
    ImplicitDefault(); // call default constructor (implicitly defined)
  }
}
</code></pre>

The class `ExplicitDefault` has a single constructor that takes no parameters.  This constructors type is known as the //default constructor//.  Notice how the constructor is called by the class name in the statement `ExplicitDefault();`  Also notice how `ImplicitDefault` is constructed with the default constructor in the statement `ImplicitDefault();`.  As long as there are no constructors defined, the default will always be defined by lightning.

<pre><code class="language-csharp" name="Custom Constructors">
class ExplicitCustom
{
  constructor(r : Real) {}
}

class ExplicitCustomAndDefault
{
  constructor() {}
  constructor(r : Real) {}
}

class Driver
{
  function MyFunction()
  {
    ExplicitCustom(); // ERROR
    ExplicitCustom(1.0);
    ExplicitCustomAndDefault();
    ExplicitCustomAndDefault(1.0);
  }
}
</code></pre>

The class `ExplicitCustom` defines a single constructor that takes a single [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md).  This means that `ExplicitCustom` cannot be default constructed, therefore the statement `ExplicitCustom();` fails to compile.  The default constructor can still be readded by explicitly defining it alongside other constructors, as shown in the class `ExplicitCustomAndDefault`.

NOTE: Explcitly defining a constructor is **not required** in Lightning as long as every data member of the class has a default constructor.

Destructors are called when all handles to an object are destroyed.  The exception is when an object is not a copy by reference type, in which case the destructor isn't called.

<pre><code class="language-csharp" name="Destructors">
struct MyStruct
{
  var Id : Integer;
  constructor(id : Integer)
  {
    this.Id = id;
  }
  destructor()
  {
    Console.WriteLine(this.Id);
  }
}

class MyClass : MyStruct {}

class Driver2
{
  [Static]
  function MyFunction()
  {
    var v1 = MyStruct(1);
    var v2 = local MyStruct(2);
    var v3 = new MyStruct(3);
    var v4 = MyClass(4);
    var v5 = new MyClass(5);
  } // end of the scope, all unreferenced objects are destroyed
}
</code></pre>
<pre><code name="Console window">
3
4
5
</code></pre>

In the example above, `MyClass` [inherits](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/inheritance.md) from `MyStruct`.  `MyClass` has the same members as `MyStruct`, and the only difference between the two is that `MyClass` is a `class`.  Observe how `3`, `4`, and `5` are printed, which means that the destructor got called on `v3`, `v4`, and `v5`.  All struct destructors were ignored, while all class destructors were called.  The one exception is `v3`, which is of the type `ref MyStruct` and has the copy `by-reference` quality.

# Related Materials
## Manual
- [Variables](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.md)
- [Functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.md)
- [memory_management](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/memory_management.md)
- [attributes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.md)
- [inheritance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/inheritance.md)
- [Static](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.md#static)

## Code Reference
- [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md) 

 
# Casting
Fundamentally, casting is converting from one type to another.  As demonstrated in the code snippet below, a [Function](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown) that takes a grade and returns pass/fail can be thought of as a conversion from a [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) to a [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown).
<pre><code class="language-csharp" name="Conversion Function">
function IsPassing(grade : Real) : Boolean
{
  if(grade >= 70)
    return true;
  else
    return false;
}
</code></pre>

The logic of that particular conversion is defined as a function and intended for a specific situation, but *cast operations* are more general-case and defined by Lightning.

# Implicit and Explicit
There are two types of casting, implicit and explicit.  Implicit casting occurs during the assignment of a variable of one type, with a value of a *different* type.  Implicit casting is a mechanism that Lightning uses when a [Variable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.markdown) of one type is set to data of another type.  Explicit casting is a mechanic used by the user with the `as` keyword.  Any cast that can happen implicitly can be done explicitly.

WARNING: Even with explicit casting, there are still *cast operations* that are invalid and will trigger compile-time exceptions.

<pre><code class="language-csharp" name="Casting Implicitly and Explicitly">
var myReal : Real = 1.0;
var myDoubleReal : DoubleReal = myReal; // implicit casting
var myInteger : Integer = myReal as Integer; // explicit casting
</code></pre>
In the example above, `myDoubleReal` is being set to `myReal`, which invokes an implicit cast from [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) to [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown).  When `myReal as Integer` is evaluated, explicit casting is invoked to convert a [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) to an [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown).  The format for explicit casting is `<value> as <new type>`.

NOTE: Explicit casting should only be used when one is aware of all of the nuances of the cast.

# Casting Between Numeric and Boolean Types
The following base data types are considerered Numeric and Boolean:
| [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown) |
| [doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.markdown) |
| [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) |
| [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown) |
| [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown) |

All *cast operations* using only these types are valid, meaning either explicit or implicit.  The code snippit below demonstates implicit casting between numeric types.

<pre><code class="language-csharp" name="Implicit Numeric Casts">
var myInteger : Integer = 1;

var myDoubleInteger : DoubleInteger = myInteger;
var myReal : Real = myInteger;
var myDoubleReal1 : DoubleReal = myInteger;

var myDoubleReal2 : DoubleReal = myDoubleInteger;
var myDoubleReal3 : DoubleReal = myReal;
</code></pre>

Notice that implicit casting is allowed when converting to a numeric set, from a smaller data size to a larger one.  The value of `myInteger` can be implicitly casted to a [doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.markdown), which holds twice the number of bits as an [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown).  The value of `myInteger` can also be implicitly casted to a [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown).  Real values can hold whole numbers and a decimal portion, whereas integers can only be whole numbers.

(NOTE)**From a Mathematics Perspective** The integer set is a subset of the real set.  For more information on mathematical sets, visit the [Wikipedia Set (Mathematics)](https://en.wikipedia.org/wiki/Set_(mathematics)) page.

## Truncation
When a real value is converted to an integer value explicitly, the value will be truncated.  This means the decimal part of the real value will be lost, and without rounding.

<pre><code class="language-csharp" name="Implicit Numeric Casts">
Console.WriteLine(1.1 as Integer);
Console.WriteLine(2.99 as Integer);
Console.WriteLine(-3.99 as Integer);
</code></pre>
<pre><code name="Console Window">
1
2
-3
</code></pre>

# Upcasting and Downcasting
When casting between classes related through [inheritance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/inheritance.markdown), one class must be a base class of the other.

<pre><code class="language-csharp" name="Classes with Inheritance">
class A {}
class B : A {}
class C : B {}
</code></pre>

The code snippet below uses the `Classes with Inheritance` snippet.
<pre><code class="language-csharp" name="Upcasting and Downcasting">
var a : A = A();
var b : B = B();
var c : C = C();

// implicit
var ba : A = b;
var ca : A = c;
var cb : B = c;

// explicit
var ab : B = a as B;
var ac : C = a as C;
var bc : C = b as C;
</code></pre>

Notice how all the implicit casts involve converting from a derived class to a base class.  This is known as **upcasting**.  **Downcasting** involves taking a base class and casting it to a derived class, which must be done explicitly.  **Downcasting** is also a type of dynamic casting, which is validated at runtime.  Observe that the objects `a`, `b`, and `c` are all references being casted, and not values.  If a base class reference is downcasted to a derived class reference and the value referenced is of the base class type, then the cast failed at runtime.  A *failed dynamic cast* will result in the value `null`.  The code snippet below uses the `Classes with Inheritance` snippet.

<pre><code class="language-csharp" name="Dynamic Casting">
var a_ref_b : A = B(); // upcast invoked implicitly
var b_ref_a : B = A() as B; // downcast invoked explicitly
var b_ref_b : B = a_ref_b as B; // downcast invoked explicitly
Console.WriteLine(a_ref_b == null);
Console.WriteLine(b_ref_a == null);
Console.WriteLine(b_ref_b == null);
</code></pre>
<pre><code name="Console Window">
false
true
false
</code></pre>

`a_ref_b` is a reference of type `A` to a value of type `B`, which uses an implicit **upcast**.  `b_ref_a` is a reference of type `B` to a value of type `A`, which uses an explicit **downcast**.  Notice how `b_ref_a` has the value `null` at runtime, the result of a //failed dynamic cast//.  On the other hand, `a_ref_b` is successfully cast since it has a value of type `B`.

# Null Casts
The value `null` can be cast to any reference type implicitly.  The code snippet below uses the `Classes with Inheritance` snippet.

<pre><code class="language-csharp" name="Null Casting">
var a1 : A = null; // implicit cast
var a2 : A = null as A; // explicit cast (unnecessary)
</code></pre>

NOTE: Interpreting `null` as an invalid state for object references is a common pattern in programming.

 # Any Casts
Any type can be cast implicitly to an [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown), and an [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown) value can be implicitly cast to any type.  The [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown) type is used as a generic reference to any instantiated class or struct.
<pre><code class="language-csharp" name="Any Casting">
var integerOne : any = 1;
var myInteger : Integer = integerOne; // any cast
var myReal : Real = integerOne; // runtime exception
</code></pre>

Notice how the attempt to cast `integerOne`, which is an [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown), to a [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown) results in a runtime exception.  An [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown) must first be cast to the type of the value it holds, even before other implicit conversions.

# Same Casts
Same casts are casts that convert a value of one type to the same type.  All same casts can be done implicitly and are unnecessary.
<pre><code class="language-csharp" name="Same Casting">
var myReal : Real = 1.0; // implicit same cast
var myInteger : Integer = 1 as Integer; // explicit same cast
</code></pre>

# Related Materials
## Manual
- [Function](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/functions.markdown)
- [Variable](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/variables_and_data_types.markdown)
- [inheritance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/inheritance.markdown)

## Code Reference
- [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)
- [doubleinteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doubleinteger.markdown)
- [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)
- [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)
- [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)
- [any](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/any.markdown) 

 
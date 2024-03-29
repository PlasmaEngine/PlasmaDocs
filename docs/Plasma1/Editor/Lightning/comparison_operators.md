# Comparison Operators

Comparison operators take two operands and evaluate to a boolean value which describes a relationship between the given values. Comparison operators are frequently used with [conditionals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/conditionals.md).

# `==` & `!=` Operators
The `==` (equality) operator compares two operands and returns `true` if they are the same and `false` if they are not. The `!=` (inequality) operator performs the inverse operation, returning `false` if they are the same and `true` if they are not.

| Left Operand | Operator | Right Operand | Result |
| `true` | `==` | `true` | `true` |
| `true` | `==` | `false` | `false` |
| `true` | `!=` | `true` | `false` |
| `true` | `!=` | `false` | `true` |

The equality operator is very useful when trying to identify unknown data, or verifying existing data.

<pre><code class="language-csharp" name="== Operator Identifying Data">
if(unknownObject == this.TargetObject)
{
  Console.WriteLine("Found Target");
}
</code></pre>

<pre><code class="language-csharp" name="== Operator Verifying Data">
if(this.Owner.Player.TeamId == hitObject.Player.TeamId)
  Console.WriteLine("Friendly Fire!");
</code></pre>

Keep in mind that the values of the operands must be exactly equal. When comparing decimal values, the differences may be very small but still exist, i.e. `3.14159 == 3.141591` will evaluate to `false`. Similarly `2.236068 == 2.23607` will evaluate to `false`, as the values differ by `0.0000002`. It is common to use an *epsilon* value (i.e. `0.0000001`) when comparing values that are more precise then the comparison needs to be.


The `!=` operator is commonly used to verify data exists before attempting to use it.
<pre><code class="language-csharp" name="!= Operator Verifying Data">
if(unknownObject != null)
{
  Console.WriteLine(`unkownObject` is valid);
  if(unknownObject.Transform != null)
    Console.WriteLine(unkownObject.Transform.Translation);
  else
    Console.WriteLine("`unkownObject` does not have a Tranform component");
}
</code></pre>

# Object Comparison
As seen in the first code block, object comparison is fairly common. However, there are a few details to be aware of when comparing objects by value vs. by reference.

NOTE: To read about the details about by-value and by-reference objects, [ read the manual page](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/constructbyvaluevsbyref.md).

## Object Comparison by Value
Take the following struct as a by-value example:

<pre><code class="language-csharp" name="ValueObj">
struct ValueObj
{
  var ValueOne : Boolean;
  var ValueTwo : Integer;
  var ValueThree : Boolean;
}
</code></pre>

In Lightning, structs are value types, so when they're compared using the `==` or `!=` operators, the value(s) within the type are what is compared. This means that the `==` and `!=` operators **cannot** be used with references to structs to determine if the operands are the same struct instance.

<pre><code class="language-csharp" name="Comparing Objects - ValueObj">
var a = ValueObj();
var b = a;
var c = ValueObj();
Console.WriteLine("a & b are equal: `a == b`");

b.ValueOne = true;
Console.WriteLine("a & b are equal: `a == b`");

Console.WriteLine("a & c are equal: `a == c`");
Console.WriteLine("b & c are equal: `b == c`");
</code></pre>
<pre><code name="Console Output">
a & b are equal: true
a & b are equal: false
a & c are equal: true
b & c are equal: false
</code></pre>

In this case, the `ValueObj` instances are constructed and compared by value. So despite `b` being a copy of `a`, when `b.ValueOne` is set to false, the value of `a.ValueOne` does not change, and the values of the two objects are no longer equal. Furthermore, it can be seen that even when `ValueObj` instance `c`, a new value type instance, is constructed, the `ValueObj` is only copied and compared by value.

## Object Comparison by Reference
Take the following class as a by-reference example:

<pre><code class="language-csharp" name="ReferenceObj">
class ReferenceObj
{
  var ValueOne : Boolean;
  var ValueTwo : Integer;
  var ValueThree : Boolean;
}
</code></pre>

In Lightning, classes are reference types, so when they're compared using the `==` or `!=` operators, what are actually compared are the addresses of the objects in memory. This means that the `==` and `!=` operators **cannot** be used with class references to determine if the operands contain the same values; instead, they reveal whether the two objects are the same class instance.

<pre><code class="language-csharp" name="Comparing Objects - ReferenceObj">
var a = ReferenceObj();
var b = a;
var c = ReferenceObj();
Console.WriteLine("a & b are equal: `a == b`");

b.ValueOne = false;
Console.WriteLine("a & b are equal: `a == b`");

Console.WriteLine("a & c are equal: `a == c`");
Console.WriteLine("b & c are equal: `b == c`");
</code></pre>
<pre><code name="Console Output">
a & b are equal: true
a & b are equal: true
a & c are equal: false
b & c are equal: false
</code></pre>

In this case, the `ReferenceObj` instances are constructed and compared by reference, so `b` is actually a copy of the reference `a` to the constructed `ReferenceObj`. This means that when `b.ValueOne` is set to `true`, the `ReferenceObj` instance that `a` references is modified, as `a` and `b` are in fact referencing the same `ReferenceObj` instance.  Furthermore, looking at `c`, one can see that when a new reference type instance is constructed, it is only copied and compared by reference, so even when two instances contain the same value(s), they will not be considered equal.


# Floating-Point Comparison

Due to floating-point error, it is best to avoid comparing two extremely precise or large values of floating-point types (such as [ Real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)) with the `==` and `!=` operators. Consider:

<pre><code class="language-csharp" name="Floating-Point Comparison, Example 1">
Console.WriteLine(2000000000.0 == 2000000042.0);
</code></pre>
<pre><code name="Console Output">
true
</code></pre>

This is not a quirk of the engine, it's a quirk of modern computing. Instead of using these operators, it is best to use a function like `Math.ApproximatelyEqual` (which can then be negated using the `!` operator to check for inequality) for floating-point types. For example, instead of something like this:
<pre><code class="language-csharp" name="Floating-Point Comparison, Example 2 (problematic)">
if (this.Transform.WorldTranslation.Y == this.JumpHeight)
{
  //
}
</code></pre>
... try something like this:
<pre><code class="language-csharp" name="Floating-Point Comparison, Example 2 (fixed)">
if (Math.ApproximatelyEqual(this.Transform.WorldTranslation.Y, this.JumpHeight, 0.01))
{
  //
}
</code></pre>

# `>` & `<` Operators
The `>` (greater than) operator returns true if the left operand is *greater than// the right operand. The `<` (less than) operator returns true if the left operand is //less than* the right operand.

| Left Operand | Operator | Right Operand | Result |
| `0` | `>` | `1` | `false` |
| `1` | `>` | `1` | `false` |
| `2` | `>` | `1` | `true` |
| `0` | `<` | `1` | `true` |
| `1` | `<` | `1` | `false` |
| `2` | `<` | `1` | `false` |

`<` is often used to compare simulation values to detemine if a threshold has failed to be reached.

<pre><code class="language-csharp" name="< Operator Checking Threshold">
if(height < 5)
  Console.WriteLine("You must be at least 5ft tall to ride this attraction");
</code></pre>

`>` is often used to compare simulation values to detemine if a threshold has been exceeded.

<pre><code class="language-csharp" name="> Operator Checking Threshold">
if(cost > 10)
  Console.WriteLine("That restaurant is not within my dinner budget");
</code></pre>

# `>=` & `<=` Operators
The `>=` (greater than or equal to) operator returns true if the left operand is *greater than **or** equal to// the right operand. The `<=` (less than or equal to) operator returns true if the left operand is //less than **or** equal to* the right operand.

| Left Operand | Operator | Right Operand | Result |
| `0` | `>=` | `1` | `false` |
| `1` | `>=` | `1` | `true` |
| `2` | `>=` | `1` | `true` |
| `0` | `<=` | `1` | `true` |
| `1` | `<=` | `1` | `true` |
| `2` | `<=` | `1` | `false` |

`<=` is often used to compare simulation values to detemine if a threshold has failed to be exceeded.

<pre><code class="language-csharp" name="< Operator Checking Threshold">
if(cost <= 10)
  Console.WriteLine("That restaurant is within my dinner budget");
</code></pre>

`>` is often used to compare simulation values to detemine if a threshold has been exceeded.

<pre><code class="language-csharp" name="> Operator Checking Threshold">
if(height >= 5)
  Console.WriteLine("You are at least 5ft tall, you may ride this attraction");
</code></pre>

# Related Materials
# Manual
- [operators_precedence_chart](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/operators_precedence_chart.md)
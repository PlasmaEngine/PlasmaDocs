# Boolean Operators

NOTE: It is highly suggested you read [conditionals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/conditionals.md) before this page, as the concepts of conditionals are used through out to demonstrate Boolean Operators.

The [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md) type has special operators that work with it.

# The Negation Operator `!`
The `!` operator, called the negation operator, is typically the simplest of the boolean operators as it changes the value of its operand to `true` if it was `false`, and changes the value to `false` if it was `true`.

<pre><code class="language-csharp" name="The ! Operator">
var a = true;
Console.WriteLine("a starts as `a`");
a = !a;
Console.WriteLine("a is negated and is now `a`");
a = !a;
Console.WriteLine("a is negated again and is now `a` again");
</code></pre>
<pre><code name="Console Output">
a starts as true
a is negated and is now false
a is negated again and is now true again
</code></pre>

# Comparison Operators
All comparison operators take a left side and right side operand and evaluate to a boolean value.

## Equality `==`
Often certain code should only run under specific conditions. The `==` operator, called the Equality operator, determines if the value of two operands are equalivalent and returns `true` or `false`.

<pre><code class="language-csharp" name="Equality Operator">
var a = true;
var b = true;
var c = false;

Console.WriteLine("a is equal to b: `a == b`");
Console.WriteLine("a is equal to c: `a == c`");
Console.WriteLine("b is equal to c: `b == c`");
Console.WriteLine("a, b, and c are equal: `a == b == c`");
</code></pre>
<pre><code name="Console Output">
a is equal to b: true
a is equal to c: false
b is equal to c: false
a, b, and c are equal: false
</code></pre>

While the Equality operator is not exclusively used with booleans it does always result in a boolean value.

|Equality | | `==` |
| **Left Operand** | **Right Operand** | **Result** |
| `true` | `true` | `true` |
| `true` | `false` | `false` |
| `false` | `true` | `false` |
| `false` | `false` | `true` |

## Inequality `!=`
The `!=` operator, called the inequality operator, is the logical inverse of the equality operator return `true` if the operands are not the equal and `false` if they are.
<pre><code class="language-csharp" name="Inequality Operator">

var a = true;
var b = true;
var c = false;

Console.WriteLine("a is not equal to b: `a != b`");
Console.WriteLine("a is not equal to c: `a != c`");
Console.WriteLine("b is not equal to c: `b != c`");
Console.WriteLine("a, b, and c are not equal: `a != b != c`");
</code></pre>
<pre><code name="Console Output">
a is not equal to b: false
a is not equal to c: true
b is not equal to c: true
a, b, and c are not equal: false
</code></pre>

Notice that `a != b != c` results in false. This is because `==` and `!=` are evaluated left to right. So first `a != b` returns `false` as both variables have a value of `true`. Because `a != b` evaluates to `false` and `c` has a value of `false` `a != b != c` is reduced to `false != c`. The reduced form evaluates to `false` since both operands have a value of `false`.

|Inequality | | `!=` |
| **Left Operand** | **Right Operand** | **Result** |
| `true` | `true` | `false` |
| `true` | `false` | `true` |
| `false` | `true` | `false` |
| `false` | `false` | `false` |

## Less Than & Greater Than `<` & `>`
The `<` and `>` operators, called the less or greater then operators respectively, evaluate if one operand has a smaller/larger value than the other.

<pre><code class="language-csharp" name="Less/Greater Than">
var i = 0;
var j = 1;
var k = 0;

Console.WriteLine("i is less than j: `i < j`");
Console.WriteLine("i is less than k: `i < k`");
Console.WriteLine("j is less than k: `j < k`");
Console.WriteLine("i is greater than j: `i > j`");
Console.WriteLine("i is greater than k: `i > k`");
Console.WriteLine("j is greater than k: `j > k`");
</code></pre>
<pre><code name="Console Output">
i is less than j: true
i is less than k: false
j is less than k: false
i is greater than j: false
i is greater than k: false
j is greater than k: true
</code></pre>

Notice that `i` is not less or greater than `k` as `0` is not less or greater than `0`.

## Less Than or Equal & Greater Than or Equal (`<=` & `>=`)
The `<=` and `>=`, called the `less than or equal to` and `greater than or equal to` operators, determine if the value of the left operand is lesser than, greater than, or equal to the right operand.

<pre><code class="language-csharp" name="Less/Greater Than">
var i = 0;
var j = 1;
var k = 0;

Console.WriteLine("i is less or equal to than j: `i <= j`");
Console.WriteLine("i is less or equal to than k: `i <= k`");
Console.WriteLine("j is less or equal to than k: `j <= k`");
Console.WriteLine("i is greater than or equal to j: `i >= j`");
Console.WriteLine("i is greater than or equal to k: `i >= k`");
Console.WriteLine("j is greater than or equal to k: `j >= k`");
</code></pre>
<pre><code name="Console Output">
i is less than or equal to j: true
i is less than or equal to k: true
j is less than or equal to k: false
i is greater than or equal to j: false
i is greater than or equal to k: true
j is greater than or equal to k: true
</code></pre>

# Logical Operators
Logical operators take a left and a right side areguement, both of which must evaluate to boolean values, and evaluates them returning another boolean value.

# and `&&`
The `&&` operator, called the `and` operator, takes two boolean values and evaluates them, returning true only if both operands evaluate to true. This can be very useful as often one may find that a condition in script may depend on two seperate factors.

<pre><code class="language-csharp" name="Nested if">
var i = true;
var j = false;

if(i)
{
  if(j)
  {
    Console.WriteLine("Both i and j are true");
  }
  else
  {
    Console.WriteLine("Inner Else: Either i or j is false");
  }
}
else
{
  Console.WriteLine("Outer Else: Either i or j is false");
}
</code></pre>
<pre><code name="Console Output">
Inner Else: Either i or j is false
</code></pre>

This can be simplified using the `&&` operator to evaluate both `i` and `j` within the same `if` statement.

<pre><code class="language-csharp" name="&&">
var i = true;
var j = false;

if(i && j)
{
  Console.WriteLine("Both i and j are true");
}
else
{
  Console.WriteLine("Either i or j is false");
}
</code></pre>
<pre><code name="Console Output">
Either i or j is false
</code></pre>

The nested `if` version of the above code does allow information about whether it is `i` or `j` which is `false` to be gathered, but in many cases the *which* doesn't matter, just that one of them is `false` is enough.

|And | | `&&` |
| **Left Operand** | **Right Operand** | **Result** |
| `true` | `true` | `true` |
| `true` | `false` | `false` |
| `false` | `true` | `false` |
| `false` | `false` | `false` |

(NOTE)**Short Circuiting the Right Side Operand**: Since logical `and` is an operator which is resolved left to right is can always be assumed that the left operand will be evaluated to either `true` or `false` before the righthand operand is evaluated at all. This is important as if the first operand does not evaluate to `true` the operator will immeidiately evaluate to `false` *short circuiting* the right side an causing it to not resolve and evaluate the expression of the right side operand at all. A good usage example is when checking object validity before accessing members such as components.

# or `||`
The `||` operator, called the `or` operator, takes two boolean values and evaluates them, returning true if either operands evaluates to true.


<pre><code class="language-csharp" name="||">
var i = true;
var j = false;

if(i || j)
{
  Console.WriteLine("Either i or j is true");
}
else
{
  Console.WriteLine("Neither i or j is true");
}
</code></pre>
<pre><code name="Console Output">
Either i or j is true
</code></pre>

|And | | `||` |
| **Left Operand** | **Right Operand** | **Result** |
| `true` | `true` | `true` |
| `true` | `false` | `true` |
| `false` | `true` | `true` |
| `false` | `false` | `false` |


# Related Materials
## Manual
- [conditionals](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/conditionals.md)

## Code Reference
- [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.md) 

 
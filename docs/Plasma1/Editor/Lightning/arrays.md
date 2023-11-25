# Arrays
[Array](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md) is a templated Lightning type used to represent an ordered list. An array is a *container* class: it contains other objects. The type of object it contains is specified between square brackets when the array is declared:

<pre><code class="language-csharp" name="Array Declaration Example">
var recentPositions = Array[Real3]();
var currentTargets = Array[Cog]();
var inputBuffer = Array[Array[Boolean]]();
</code></pre>

When an array is created, by default, it has no elements, but its initial size can be specified, and, optionally, the initial value of each element can be provided as well:

<pre><code class="language-csharp" name="Array Initialization Example 1">
var emptyArray           = Array[Integer]();
var eightDefaultIntegers = Array[Integer](8);
var eightFives           = Array[Integer](8, 5);

Console.WriteLine(emptyArray);
Console.WriteLine(eightDefaultIntegers);
Console.WriteLine(eightFives);
</code></pre>
<pre><code name="Console Window">
{}
{0, 0, 0, 0, 0, 0, 0, 0}
{5, 5, 5, 5, 5, 5, 5, 5}
</code></pre>

NOTE: When specifying the initial value for an array's elements in this manner, take note that one such element is constructed, and then it is duplicated as necessary to fill the array. If the type stored in the array is a value type, this will result in the construction of additional elements, but if it is a reference type, then each additional element will be a by-reference copy of the first. This may lead to unexpected behavior when modifying the array's contents later. If explicit copies of a reference type object are desired, they should be created and added after construction.

Additionally, an array can be initialized with an initializer list:

<pre><code class="language-csharp" name="Array Initialization Example 2">
var a = Array[String]() { "abc", "def", "ghi", "jkl" };

Console.WriteLine(a);
</code></pre>
<pre><code class="language-csharp" name="Console Window">
{abc, def, ghi, jkl}
</code></pre>

# Array Access

Array elements can be accessed for reading or writing using the **indexing operator**, `[]`. Array indexing in Lightning is **plasma-based** (the very first element in an array has an index of 0):

<pre><code class="language-csharp" name="Access Example">
var words = Array[String]()
{
  "the",    // element 0
  "quick",  // element 1
  "brown",  // element 2
  "fox",    // element 3
};

var chosenWord = words[1];      // reading element 1
Console.WriteLine(chosenWord);

words[2] = "polka-dotted";      // writing element 2
Console.WriteLine(words);
</code></pre>

<pre><code name="Console Window">
quick
{the, quick, polka-dotted, fox}
</code></pre>

Attempting to access a negative index or an index that is greater than or equal to the array's [Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#array-size) will throw a Lightning exception.

# Adding to and Removing from Arrays

Lightning arrays are //dynamic//: that is, the number of elements in an array is not fixed, so elements can be added or removed after the array is created.

## Adding

The most basic way to add an element to an array is with the [ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#add-void) method, which puts the element at the end of the array:

<pre><code class="language-csharp" name="Add Example">
var greetings = Array[String]()
{
  "hello",
  "bonjour",
  "yo",
};
Console.WriteLine(greetings);

greetings.Add("howdy");
Console.WriteLine(greetings);
</code></pre>

<pre><code name="Console Window">
{hello, bonjour, yo}
{hello, bonjour, yo, howdy}
</code></pre>

The [ Push](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#push-void) method is functionally identical to Add for arrays, and they may be used interchangeably.

Adding to the end is generally the fastest way of adding to an array, but it is possible to insert an element at any valid position within an array via the [ Insert](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#insert-void) method:

<pre><code class="language-csharp" name="Insert Example">
var digitsOfE = Array[Integer]() { 2, 7, 1, 2, 8 };
Console.WriteLine(digitsOfE);

digitsOfE.Insert(3, 8); // adds an 8 so that its new index is 3
Console.WriteLine(digitsOfE);
</code></pre>

<pre><code name="Console Window">
{2, 7, 1, 2, 8}
{2, 7, 1, 8, 2, 8}
</code></pre>

NOTE: Insert is less efficient than Add because it requires all the elements following the given index to be shifted toward the back of the array to make room for the new element. If the proper position of a new element is at the end of the array, or if the order of the elements is irrelevant, Add should generally be used instead of Insert.

## Removing

The most basic way to remove an element from an array is with the [ Pop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#pop-plasma-engine-document) method, which shrinks the array by one from the end:

<pre><code class="language-csharp" name="Pop Example">
var taskList = Array[String]()
{
  "make the game fun",
  "UI overhaul",
  "create placeholder SFX",
  "vacuum the break room",
};
Console.WriteLine(taskList);

taskList.Pop();
Console.WriteLine(taskList);
</code></pre>

<pre><code  name="Console Window">
{make the game fun, UI overhaul, create placeholder SFX, vacuum the break room}
{make the game fun, UI overhaul, create placeholder SFX}
</code></pre>

As with adding, removing from the end is fast, but it is also possible to remove an element at an arbitrary valid index via the [ RemoveAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeat-void) and [ RemoveSwap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeswap-void) methods.

**RemoveAt** removes the element that is found at the given index, and preserves the order of the remaining elements:

<pre><code class="language-csharp" name="RemoveAt Example">
var commonLetters = Array[String]()
{
  "e",  // 0
  "t",  // 1
  "a",  // 2
  "x",  // 3 (this one doesn't belong)
  "o",  // 4
  "i",  // 5
  "n",  // 6
};
Console.WriteLine(commonLetters);

commonLetters.RemoveAt(3);
Console.WriteLine(commonLetters);
</code></pre>

<pre><code  name="Console Window">
{e, t, a, x, o, i, n}
{e, t, a, o, i, n}
</code></pre>

NOTE: RemoveAt is less efficient than Pop because it causes all the elements following the given index to be shifted toward the front of the array to close the gap following the removal. If the element to be removed is the last element in the array, Pop should be used instead of RemoveAt.

Alternatively, there is another option if the order of elements is irrelevant. **RemoveSwap** first swaps the element at the given index with the last element in the array, and then Pops the element from the end. The order of the remaining elements is thus *not* preserved:

<pre><code class="language-csharp" name="RemoveSwap Example">
var animals = Array[String]()
{
  "tardigrade",   // 0
  "aardwolf",     // 1
  "pile of dirt", // 2 (this one doesn't belong)
  "sponge",       // 3
  "plesiosaur",   // 4
};
Console.WriteLine(animals);

animals.RemoveSwap(2);
Console.WriteLine(animals);
</code></pre>

<pre><code  name="Console Window">
{tardigrade, aardwolf, pile of dirt, sponge, plesiosaur}
{tardigrade, aardwolf, plesiosaur, sponge}
</code></pre>

Though RemoveSwap does not preserve element order, it is essentially just as efficient as Pop.

It is also possible to remove a known element with an unknown index. [ RemoveFirst](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removefirst-plasma-engine) finds an array's first element that matches the given value and then removes it, preserving the order of the remaining elements:

<pre><code class="language-csharp" name="RemoveFirst Example">
var data = Array[Integer]()
{
  0,
  4,
  1,
  -1, // (this one doesn't belong)
  2,
};
Console.WriteLine(data);

data.RemoveFirst(-1);
Console.WriteLine(data);
</code></pre>
<pre><code  name="Console Window">
{0, -1, 4, 1, 2}
{0, 4, 1, 2}
</code></pre>

To find and remove *all* elements that match a given value, use the [ RemoveAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeall-plasma-engine-do) method:

<pre><code class="language-csharp" name="RemoveAll Example">
var waterfowl = Array[String]()
{
  "duck",
  "duck",
  "duck",
  "duck",
  "goose",
};
Console.WriteLine(waterfowl);

waterfowl.RemoveAll("duck");
Console.WriteLine(waterfowl);
</code></pre>

<pre><code  name="Console Window">
{duck, duck, duck, duck, goose}
{goose}
</code></pre>

NOTE: Both RemoveFirst and RemoveAll require searching the array and comparing each element with the given value, which makes them even slower than RemoveAt. In certain situations, such as a deeply nested loop, or when element comparison is slow, this performance difference may be significant.

Finally, to remove all of the elements from an array, use the [ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#clear-void) method:

<pre><code class="language-csharp" name="Clear Example 1">
var inventory = Array[String]()
{
  "car keys",
  "cell phone",
  "screwdriver",
  "leaflet",
  "crumpled note",
};
Console.WriteLine(inventory);

inventory.Clear();
Console.WriteLine(inventory);
</code></pre>
<pre><code  name="Console Window">
{car keys, cell phone, screwdriver, leaflet, crumpled note}
{}
</code></pre>

NOTE: The act of removing an item from an array does not itself delete the item. If one or more external references to an element exist, then that element will persist if it is removed from an array:

<pre><code class="language-csharp" name="Clear Example 2">
var arrayContainer = Array[Array[Real]]();

var array0 = Array[Real]() { 1, 2, 3 };
var array1 = Array[Real]() { 1.61803, 2.71828, 3.14159 };

arrayContainer.Add(array0);
arrayContainer.Add(array1);

Console.WriteLine("arrayContainer before Clear: `arrayContainer`");

arrayContainer.Clear();
Console.WriteLine("arrayContainer after Clear: `arrayContainer`");
Console.WriteLine("array0 after Clear: `array0`");
Console.WriteLine("array1 after Clear: `array1`");
</code></pre>

<pre><code  name="Console Window">
arrayContainer before Clear: {{1, 2, 3}, {1.61803, 2.71828, 3.14159}}
arrayContainer after Clear: {}
array0 after Clear: {1, 2, 3}
array1 after Clear: {1.61803, 2.71828, 3.14159}
</code></pre>

# Reference Type

In Lightning, **Array** is a //reference type//. Be aware of this when making copies. When setting one array variable to equal another existing array using the assignment operator, `=`, a copy is not constructed; rather, the first just ends up pointing to the second. In such a case, modifying the array through one of the two references will appear to modify both, because they are in fact one array. To create a copy, the [ Copy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#copy-array-t) method should be used:

<pre><code class="language-csharp" name="Array Reference Type Example">
var firstExample = Array[Integer]() { 0, 1, 2, 3, 4, 5, 6, 7 };
Console.WriteLine("firstExample, before copy and clear:  `firstExample`");

var naiveCopy = firstExample;
// this doesn't actually make a copy, it just points the variable
// "naiveCopy" to the same array that "firstExample" points to
naiveCopy.Clear();
// thus, this line clears the original array

Console.WriteLine("firstExample, after copy and clear:   `firstExample`");

var secondExample = Array[Integer]() { 7, 6, 5, 4, 3, 2, 1, 0 };
Console.WriteLine("secondExample, before copy and clear: `secondExample`");

var properCopy = secondExample.Copy();
// the Copy method should be used to clone an array
properCopy.Clear();

Console.WriteLine("secondExample, after copy and clear:  `secondExample`");
</code></pre>

<pre><code  name="Console Window">
firstExample, before copy and clear:  {0, 1, 2, 3, 4, 5, 6, 7}
firstExample, after copy and clear:   {}
secondExample, before copy and clear: {7, 6, 5, 4, 3, 2, 1, 0}
secondExample, after copy and clear:  {7, 6, 5, 4, 3, 2, 1, 0}
</code></pre>

# Looping Over Arrays

As arrays are ordered sequences of objects, they lend themselves naturally to use in [ loops](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.md): in each loop iteration, the next element of the array can be accessed, modified, copied, etc.

## For Loops

The most basic way to loop over an array is by using a [ for loop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.md#for-loop). This takes advantage of the fact that an array contains its [ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#count-plasma-engine-docume), or number of elements, as a property:

<pre><code class="language-csharp" name="For Loop Example">
var numbers = Array[Integer]() { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, };

Console.WriteLine("Squares:");

for (var i = 0; i < numbers.Count; ++i)
{
  var currentNumber = numbers[i];
  
  Console.WriteLine(currentNumber * currentNumber);
}
</code></pre>
<pre><code  name="Console Window">
Squares:
0
1
4
9
16
25
36
49
64
81
</code></pre>

## For Each Loops

Another way to iterate through an array is to use a [ foreach loop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.md#for-each-loop):

<pre><code class="language-csharp" name="For Each Loop Example">
var numbers = Array[Integer]() { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, };

Console.WriteLine("Cubes:");

foreach (var number in numbers)
{
  Console.WriteLine(number * number * number);
}
</code></pre>
<pre><code  name="Console Window">
Cubes:
0
1
8
27
64
125
216
343
512
729
</code></pre>

# Array Size

A Lightning array keeps track of two different size-related properties: [ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#count-plasma-engine-docume) and [ Capacity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#capacity-plasma-engine-doc). When an array is initialized, it is allotted just enough memory to store the given number of elements. If an element is added when it doesn't have enough allocated space for another one, the array is automatically expanded so that it can fit more elements. An array's **Count** is the number of elements that have been added to it (or were placed there on initialization); its **Capacity** is the number of elements that could possibly fit in it before it needs to grow again:

<pre><code class="language-csharp" name="Count and Capacity Example">
var array = Array[Integer]();

for (var i = 0; i < 10; ++i)
{
  Console.WriteLine("Count: `array.Count` | Capacity: `array.Capacity`");
  array.Add(i);
}

Console.WriteLine("Count: `array.Count` | Capacity: `array.Capacity`");
</code></pre>
<pre><code  name="Console Window">
Count: 0 | Capacity: 0
Count: 1 | Capacity: 2
Count: 2 | Capacity: 2
Count: 3 | Capacity: 3
Count: 4 | Capacity: 4
Count: 5 | Capacity: 6
Count: 6 | Capacity: 6
Count: 7 | Capacity: 9
Count: 8 | Capacity: 9
Count: 9 | Capacity: 9
Count: 10 | Capacity: 13
</code></pre>

NOTE: If an element can be added to an array without it having to grow, it can be done very quickly, but expanding an array is potentially costly. In certain situations, such as a deeply nested loop, it may be beneficial to consider an array's Capacity before adding to it. Likewise, if the desired maximum size of an array is known ahead of time, space can be pre-allocated without adding any elements using the [ Reserve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#reserve-void) method.

# Sorting Arrays

Lightning arrays may be sorted using the [ Sort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#sort-void) method. Sorting an array may put it in, say, increasing or decreasing order, in the case of an array of Integer or another numeric type, or in alphabetical order, in the case of a String array, or some other order via some more abstract or complex set of criteria.

**Sort** sorts an array using the given comparison function. In many cases, this is something the user creates, though some types, such as [ String](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md), provide static functions that can be used with the Sort method:

<pre><code class="language-csharp" name="String Sorting Example">
var strings = Array[String]();

strings.Add("hi");
strings.Add("greetings");
strings.Add("nice to see you");
strings.Add("good morning");

Console.WriteLine(strings);

strings.Sort(String.Compare); // the Compare function is passed as a delegate

Console.WriteLine(strings);
</code></pre>
<pre><code  name="Console Window">
{hi, greetings, nice to see you, good morning}
{good morning, greetings, hi, nice to see you}
</code></pre>

A user-created array comparison function should take as arguments two objects of the type stored in the array. It should compare them in some relevant manner and return either a Boolean or an Integer that tells the Sort function what to do with the two array elements: the Boolean should be true if first item should be sorted before the second, and false otherwise; the Integer should be negative if the first item should be sorted before the second, and nonnegative otherwise.

Consider these two classes: one defining some data for an adventurer and some static functions that can be used to sort an array of Adventurers, and another containing an array of Adventurers and a method that returns a string representation of that array:

<pre><code class="language-csharp" name="Sorting Example Classes">
class Adventurer
{
  var Name : String;
  var HP : Integer;
  var Height : Real;  // in meters
  
  [Static] function CompareNames(a : Adventurer, b : Adventurer) : Integer
  {
    return String.Compare(a.Name, b.Name);
  }
  
  [Static] function CompareHPsAscending(a : Adventurer, b : Adventurer) : Integer
  {
    if (a.HP < b.HP)  return -1;
    if (a.HP == b.HP) return 0;
    return 1;
  }
  
  [Static] function CompareHeightsAscending(a : Adventurer, b : Adventurer) : Integer
  {
    if (a.Height < b.Height)  return -1;
    if (a.Height == b.Height) return 0;
    return 1;
  }
  
  [Static] function CompareNameLengthsThenAlpha(a : Adventurer, b : Adventurer) : Integer
  {
    var aNameLength = a.Name.ComputeRuneCount();
    var bNameLength = b.Name.ComputeRuneCount();
    
    if (aNameLength < bNameLength) return -1;
    if (aNameLength > bNameLength) return 1;
    return Adventurer.CompareNames(a, b);
  }
}

class Party
{
  var Roster : Array[Adventurer] = Array[Adventurer]();
  
  function ToString() : String
  {
    var sb = StringBuilder();
    sb.Write("{ ");
    
    for (var i = 0; i < this.Roster.Count; ++i)
    {
      var member = this.Roster[i];
      sb.Write(member.Name);
      
      if (i < this.Roster.LastIndex)
        sb.Write(", ");
    }
    
    sb.Write(" }");
    return sb.ToString();
  }
}
</code></pre>

These classes can be used to illustrate how to sort objects of custom classes:

<pre><code class="language-csharp" name="Custom Class Sorting Example">
var party = Party()
{
  Roster = Array[Adventurer]()
  {
    Adventurer() { Name = "Trevor", HP = 14, Height = 1.75 },
    Adventurer() { Name = "Nathan", HP = 17, Height = 1.80 },
    Adventurer() { Name = "Joshua", HP = 14, Height = 1.85 },
    Adventurer() { Name = "Josh",   HP = 17, Height = 1.68 },
    Adventurer() { Name = "Ryan",   HP = 25, Height = 1.83 },
    Adventurer() { Name = "Dane",   HP = 9,  Height = 1.70 },
    Adventurer() { Name = "Andrea", HP = 17, Height = 1.65 },
  }
};

Console.WriteLine("Default order:            `party.ToString()`");
party.Roster.Sort(Adventurer.CompareNames);
Console.WriteLine("Alphabetical order:       `party.ToString()`");
party.Roster.Sort(Adventurer.CompareHPsAscending);
Console.WriteLine("HP order, ascending:      `party.ToString()`");
party.Roster.Sort(Adventurer.CompareHeightsAscending);
Console.WriteLine("Height order, ascending:  `party.ToString()`");
party.Roster.Sort(Adventurer.CompareNameLengthsThenAlpha);
Console.WriteLine("Name lengths then alpha:  `party.ToString()`");
</code></pre>
<pre><code  name="Console Window">
Default order:            { Trevor, Nathan, Joshua, Josh, Ryan, Dane, Andrea }
Alphabetical order:       { Andrea, Dane, Josh, Joshua, Nathan, Ryan, Trevor }
HP order, ascending:      { Dane, Joshua, Trevor, Andrea, Josh, Nathan, Ryan }
Height order, ascending:  { Andrea, Josh, Dane, Trevor, Nathan, Ryan, Joshua }
Name length then alpha:   { Dane, Josh, Ryan, Andrea, Joshua, Nathan, Trevor }
</code></pre>

Note that the `CompareNameLengthsThenAlpha` function sorts Adventurers in ascending order of the lengths of their names, except where there is a tie, in which case it sorts in ascending alphabetical order instead.

# Array Properties

## All

[ All](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#all-arrayrange-t-key-rea) converts the array into an ArrayRange. In Lightning, Arrays can be implicitly cast to ArrayRanges, so it is typically not necessary to use this property.

## Count and Capacity

[ Count](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#count-plasma-engine-docume) and [ Capacity](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#capacity-plasma-engine-doc) get the number of elements in the array, and its potential capacity to hold elements, respectively. They are discussed in detail [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#array-size).

## LastIndex

[ LastIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#lastindex-plasma-engine-do) gets the index of the last element in the array. It is always one less than Count (even when Count is 0).

# Array Methods

## Add, Push, and Insert

The [ Add](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#add-void) method expands an array so that the given element is the last item in it. The [ Push](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#push-void) method is identical to Add, and exists only for legacy purposes. The [ Insert](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#insert-void) method expands an array so that the given element is at the given index in it.

All of these methods are discussed in detail [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#adding).

## Pop, RemoveAt, RemoveSwap, RemoveFirst, RemoveAll, and Clear

The [ Pop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#pop-any) method removes the last item from an array. The [ RemoveAt](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeat-void) method removes from an array the element found at the given index. The [ RemoveSwap](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeswap-void) method removes from an array the element found at the given index and swaps the last item in the array to that newly-vacated index. The [ RemoveFirst](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removefirst-plasma-engine) method removes from an array the first element that matches the given object. The [ RemoveAll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#removeall-plasma-engine-do) method removes from an array every element that matches the given object. The [ Clear](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#clear-void) method removes all the elements from an array.

All of these methods are discussed in detail [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#removing).

## Copy

The [ Copy](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#copy-array-t) method returns a new array that is a copy of the original. This method should be used to create a clone of an array that is to be modified separately without affecting the original. Because **Array** is a reference type, this cannot be done merely with the assignment operator, as shown [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#reference-type).

## FindFirstIndex

The [ FindFirstIndex](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#findfirstindex-plasma-engi) method returns the index of the first occurrence in an array of a given object. This method compares value types by comparing their data, and it compares reference types by comparing their handles. If the given object is not found, it returns `-1`:

<pre><code class="language-csharp" name="FindFirstIndex Example">
var valueType0 = Integer2(1, 2);
// Integer2 is a value type
var valueType1 = Integer2(valueType0);
// valueType1 is a data-wise copy of valueType0
var arrayOfValueType = Array[Integer2]() { valueType0 };
Console.WriteLine(arrayOfValueType.FindFirstIndex(valueType1));
// valueType1 is found because its data is identical to valueType0

var referenceType0 = Array[Integer]() { 0, 1, 1, 2, 3, 5, 8 };
// Array[Integer] is a reference type
var referenceType1 = referenceType0.Copy();
// referenceType1 is a data-wise copy of referenceType0
var arrayOfReferenceType = Array[Array[Integer]]() { referenceType0 };
Console.WriteLine(arrayOfReferenceType.FindFirstIndex(referenceType1));
// referenceType1 is not found because its handle is not found in the array
</code></pre>
<pre><code  name="Console Window">
0
-1
</code></pre>

## Get and Set

The [ Get](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#get-plasma-engine-document) method returns the array element at the given index. The [ Set](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#set-void) method writes the given object to the given index. These methods are called when the **indexing operator**, `[]`, is used:

<pre><code class="language-csharp" name="Get Example">
var aStates = Array[String]() { "alabama", "nebraska", "arizona", "kansas" };
Console.WriteLine(aStates.Get(0));
Console.WriteLine(aStates[2]);  // this is reading, so Get is called

aStates.Set(1, "alaska");
aStates[3] = "arkansas";        // this is writing, so Set is called
Console.WriteLine(aStates);
</code></pre>
<pre><code  name="Console Window">
alabama
arizona
{alabama, alaska, arizona, arkansas}
</code></pre>

## Range

The [ Range](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#range-arrayrange-t) method returns an ArrayRange containing the specified range of elements, beginning with the given start index and including the given element count:

<pre><code class="language-csharp" name="Range Example">
var primes = Array[Integer]() { 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, };  // etc.
var primeSubset = primes.Range(4, 5);

foreach (var prime in primeSubset)
{
  Console.WriteLine(prime);
}
</code></pre>
<pre><code  name="Console Window">
11
13
17
19
23
</code></pre>

## Resize and Reserve

The [ Resize](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#resize-void) method resizes an array so that its new Count is the given value. If the given count value is greater than the array's old Count, then new elements are constructed and added to the end of the array. This method can take an optional default value parameter, which is used to set the value of these new elements; if this is not specified, then the type default for the type stored in the array will be used instead:

<pre><code class="language-csharp" name="Resize Example 1">
var iceCreamServings = Array[String]()
{
  "cookies 'n cream",
  "pistachio",
  "neapolitan",
};
Console.WriteLine(iceCreamServings);

iceCreamServings.Resize(5, "vanilla");
Console.WriteLine(iceCreamServings);

iceCreamServings.Resize(6);
Console.WriteLine(iceCreamServings);
</code></pre>
<pre><code  name="Console Window">
{cookies 'n cream, pistachio, neapolitan}
{cookies 'n cream, pistachio, neapolitan, vanilla, vanilla}
{cookies 'n cream, pistachio, neapolitan, vanilla, vanilla, (null) String}
</code></pre>

If the given count value is less than the array's old Count, then enough elements will be removed from the end of the array to bring its Count to the new value:

<pre><code class="language-csharp" name="Resize Example 2">
var cubes = Array[Integer]() { 0, 1, 8, 27, 64, 125, 216, 343, 512, 729, };
Console.WriteLine(cubes);

cubes.Resize(4);
Console.WriteLine(cubes);
</code></pre>
<pre><code  name="Console Window">
{0, 1, 8, 27, 64, 125, 216, 343, 512, 729}
{0, 1, 8, 27}
</code></pre>

As with all cases of changing an array's size, if Resize raises an array's Count past its Capacity, more space is allocated to accommodate its new size. Since this can affect performance in certain situations, it may be beneficial to change an array's Capacity before any resizing is done. The [ Reserve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#reserve-void) method sets an array's Capacity to the given value, allocating more space as necessary.

## Sort

The [ Sort](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md#sort-void) method sorts an array using the given comparison function. Typically, this is something the user provides, though some types, such as [ String](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md), provide static functions that can be used with the Sort method. Array sorting is discussed in depth [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/arrays/.md#sorting-arrays).

# Related Materials

## Manual
- [ Strings](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings.md)
- [ Classes and Structs](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md)
- [ Looping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.md)

## Code Reference
- [ Array](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/array_t.md)
- [ Integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.md)
- [ Real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)
- [ String](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/string.md) 

 
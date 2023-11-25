# Construct by value vs by ref

(NOTE)**Advanced Users Only**: The use of the **new** and **local** [keywords](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.md) __**is not something most users need to be concerned with**__, as it is almost entirely #deprecated. Heap or stack allocation is almost always handled automatically by the engine based off whether the constructed type is a class or struct, however, **new** and **local** still remain in the language for explicit allocation practices. Users attemptting to use **new** or **local** keywords should be aware that they override the standard allocation functionality of Lightning, but reference counted garbage collection will still happen for objects explicitly constructed with **new** and **local**.

# Local

When working with **by-value** types that have constructors, such as structs or more complex stack primitive data types, the keyword **local** may be used:

<pre><code class="language-csharp">
  var up : Real3 = local Real3(0.0, 1.0, 0.0);
  var stackStructInstance : CustomStruct = local CustomStruct();
</code></pre>

The compiler will infer the use of local for by-value types:
<pre><code class="language-csharp">
  // This is also valid.
  var up : Real3 = Real3(0.0, 1.0, 0.0);
  var stackStructInstance : CustomStruct = CustomStruct();
</code></pre>

# New

When working with [classes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md), references, or other or anything located on the heap with a constructor, use the **new** keyword:

<pre><code class="language-csharp">
  var heapObject : CustomClass = new CustomClass();
  var heapStructInstance : CustomStruct = new CustomStruct();
</code></pre>

Once again the compiler will infer the use of new for **by-ref** types:

<pre><code class="language-csharp">
    // This is also valid.
    var heapObject : CustomClass = CustomClass();
</code></pre>

Since structs are by-value, in order to get a reference you **must** specify new.

<pre><code class="language-csharp">
    // This does not compile
    var heapStructInstance : CustomStruct = CustomStruct();
</code></pre>

<pre><code class="language-csharp">
      The value being assigned to 'heapStructInstance' must be of type 'CustomStruct'. Its type is 'CustomStruct'.
</code></pre>

# Related Material
## Manual
- [keywords](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/keywords.md)
- [classes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/classes.md)
- [memory_management](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/memory_management.md) 

 
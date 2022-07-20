# Bound Types

NOTE: All code written here assumes `using namespace Lightning`

Bound types are created through the [ | LibraryBuilder]. This article will cover particular areas of interest on a bound type.

 #  Enumerating Members

To loop through all properties on a type, you can use the `AllProperties` array. The array stores both Property objects and Fields (which inherit from Property). The order of `AllProperties` is the order it was defined in, making it ideal for displaying properties on a property-grid or serialization (turns out users really hate it when the properties are in the wrong order). The containers we use in Lightning are range based containers, so the typical way you iterate through them is not the same as the STL. The method `all()` on Array will return a range (basically a struct that stores the STL equivalent of the `begin()` and `end()`. To walk the range, first check if its `empty()` then call `front()` to get the current value. At the end of the loop, call `popFront()` to iterate to the next item.

<pre><code class="language-csharp">
PropertyArrayRange range = boundType->AllProperties.all();

while (range.empty() == false)
{
  Property* property = range.front();

  // We can use DynamicCast to see if this is a field
  Field* field = TypeBinding::DynamicCast<Field*>(property);
  if (field != nullptr)
  {
    // ...
  }

  range.popFront();
}
</code></pre>

You can also use a built in 'for each' helper macro that wraps this behavior:

<pre><code class="language-csharp">
LightningForEach(Property* property, boundType->AllProperties.all())
{
  // Do something with 'property'
}
</code></pre>

 #  Handle Manager
ToStringFunction BaseType 

 

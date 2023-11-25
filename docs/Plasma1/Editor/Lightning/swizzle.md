# Swizzle
**Swizzling** is accessing the values within vector types ([ Real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md), [ Integer3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer3.md), etc.) in any order. The term *swizzling* originated as the name for a technique used for doing the same thing, but within shaders.

 # Understanding a Swizzle
To swizzle a vector, refer to its values as if they were data members, using the letters `X`, `Y`, `Z`, and `W` for the corresponding elements. These can be combined in any permutation or combination.

<pre><code class="language-csharp">
var a = Real3(0,1,2);
Console.WriteLine("Example 1: a.X: `a.X`");
Console.WriteLine("Example 2: a.XYZ: `a.XYZ`");
Console.WriteLine("Example 3: a.XY: `a.XY`");
Console.WriteLine("Example 4: a.YX: `a.YX`");
Console.WriteLine("Example 5: a.XXY: `a.XXY`");
Console.WriteLine("Example 6: a.ZYXZ: `a.ZYXZ`");
</code></pre>
<pre><code class="language-csharp">
Example 1: a.X: 0
Example 2: a.XYZ: (0, 1, 2)
Example 3: a.XY: (0, 1)
Example 4: a.YX: (1, 0)
Example 5: a.XXY: (0, 0, 1)
Example 6: a.ZYXZ: (2, 1, 0, 2)
</code></pre>

In this example `a` is a simple [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md):

- Example 1 constructs a [Real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md) containing the value of `a.X`
- Example 2 constructs a [by-value](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/constructbyvaluevsbyref.md) copy of `a`.
- Example 3 constructs a [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md) containing the `X` and `Y` values of `a`. 
- Example 4 constructs a [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md) with `X` as the value of `a.Y`, and `Y` as the value of `a.X`.
- Example 5 constructs a [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md) where the `X` and `Y` are set to the value of `a.X` and `Z` is set to the value of `a.Y`.
- Example 6 constructs a [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md) with the same `X`, `Y`, and `Z` values as the original vector `a`, but whose `W` value is the value of `a.Z`.

 # Assigning With Swizzles
Extracting portions of a vector as seen above is a fairly common operation even outside of shader development. An example may be centering the camera object while not affecting its zoom in a 2D game.

<pre><code class="language-csharp">
//0 out the XY axis and maintain the Z axis values
var cameraOffset = this.Camera.Transform.LocalTranslation;
cameraOffset.XY = Real2.Zero;
this.Camera.Transform.LocalTranslation = cameraOffset;
</code></pre>
If we tried to assign into the swizzle constructed by-value from the member variable, however, it would not work:

<pre><code class="language-csharp">
this.Camera.Transform.LocalTranslation.XY = Real2();
</code></pre>

In this example `.XY` returns a by-value copy of the `LocalTranslation`'s `X` and `Y` values as a [Real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md). So in this example when we assign the `Real2()` into it we are assigning into a copy instead of the member variable itself.

 # Related Materials
 ## Manual
- [constructbyvaluevsbyref](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/constructbyvaluevsbyref.md)
- [properties](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/properties.md)

 ## Reference
- [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.md)
- [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)
- [real4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4.md)
- [transform](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md)

 
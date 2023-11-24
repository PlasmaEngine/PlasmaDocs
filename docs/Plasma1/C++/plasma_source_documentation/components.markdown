# Component Example

The following example guides you through making a component in C++ and exposing it to Plasma so that it can be added to a Cog, serialized, and interact with other components.

The bare minimum requirements for making a component are as follows:
- You must publicly inherit from Component
- You must use the PlasmaDeclareType macro within the public section of the class
- You must implement the InitializeMeta function and bind the base Component class
- Our macros currently expect the component to be within the Plasma namespace

Within the `CustomComponent.hpp` header file:

<pre><code class="language-csharp">
# pragma once


namespace Plasma
{
  class CustomComponent : public Component
  {
  public:
    PlasmaDeclareType(CustomComponent);
    static void InitializeMeta(MetaType* meta);
  };
}
</code></pre>
It is our coding style to not tab in the namespace. We also generally rely upon all compilers supporing #pragma once (though you can use include guards if you wish).

Within the `CustomComponent.cpp` file:

<pre><code class="language-csharp">
# include "Precompiled.hpp"

#include "CustomComponent.hpp"

namespace Plasma
{
  PlasmaDefineType(CustomComponent);
  void CustomComponent::InitializeMeta(MetaType* meta)
  {
    BindBase(Component);
    BindSetup(SetupMode::DefaultSerialization);
  }
}
</code></pre>

The inclusion of `Precompiled.hpp` is only required if your project is using precompiled headers. All projects within Plasma have this option enabled.

The `PlasmaDeclareType` macro within the hpp file must be matched by `PlasmaDefineType` in the cpp file. These macros create a reflection `MetaType` for your class so that we can use it within script, create it via a factory, and display it in a property grid. For more information on meta binding, visit the [meta_binding](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++plasma_source_documentation/meta_binding.markdown) section.

`InitializeMeta` is called once when your component's `MetaType` gets initialized. `BindBase` tells your type that it inherits from the Component class. The `BindSetup` call with `DefaultSerialization` lets the engine know that when we create your component from a factory we'll immediately set all your member variables to their default values via the SerializeNameDefault macro (see Serialization below).

Last but not least, we must register our component with the factory and ensure that all the meta/reflection information is also initialized. This is done with one simple macro call to `RegisterComponent(CustomComponent);`. This call should be made within your project's initialization area. For example in the Engine project you would add `RegisterComponent` within `Engine\Initialization.cpp`. The easiest way to find where to initialize a component within a particular project is to look for another component defined within that project and then find its `RegisterComponent(X)` call.

Component Interface
-------------------
Within the component there are a few virtual functions which can be overridden.

- `Serialize` which is responsible for saving and loading your component
- `Initialize` which will be run once upon your component being added or loaded (after `Serialize`)
- `OnAllObjectsCreated` which is run after all objects within a context have had `Initialize` called upon them

  - For example, when loading a level
  - Or when creating an archetype (all objects within that archetype)

- `DebugDraw` will be called when your object is selected (use the `gDebugDrawer` interface)
- `OnDestroy` which will be called when your component is removed or the object is being destructed

  - Be very careful with this event, as there are many unsafe things you can do here
  - Accessing another component can be unsafe
  - Accessing another object (such as a child)
  - Creating an object here, etc

Add the following code to `CustomComponent.hpp` right after `InitializeMeta`:

<pre><code class="language-csharp">
// These functions are in the order they will be invoked:
void Serialize(Serializer& stream) override;
void Initialize(CogInitializer& initializer) override;
void OnAllObjectsCreated(CogInitializer& initializer) override;
void DebugDraw() override;
void OnDestroy(uint flags) override;
</code></pre>

You may implement these functions as you see fit. Empty implementations are OK, and they do NOT need to invoke the base class version of the function.

The following includes some common example implementations of the above functions:

<pre><code class="language-csharp">
void CustomComponent::InitializeMeta(MetaType* meta)
{
  BindBase(Component);
  BindSetup(SetupMode::DefaultSerialization);
  
  // This means we require the component Transform
  // before our component can be added
  // This also guarantees that it is safe to hold onto mTransform
  BindDependency(Transform);
  
  BindMemberProperty(mLives);
  BindMemberEnumProperty(ButtonState, mState);
  
  // If we had a GetSize and SetSize...
  BindGetSetProperty(Size);
  
  // Binding resources currently requires both Get/Set functions
  // For example, if we had a GetFace and SetFace which took a Material...
  BindGetSetResourceProperty(Material, Face);

  // These methods will be callable by script
  BindMethod(Speak);
}
</code></pre>
<pre><code class="language-csharp">
void CustomComponent::Serialize(Serializer& stream)
{
  // Our serialization handles both directions (saving and loading)
  SerializeNameDefault(mLives, 9);
  SerializeEnumName(ButtonState, mState);
  SerializeResourceName(mFace, MaterialManager);
}
</code></pre>
<pre><code class="language-csharp">
void CustomComponent::Initialize(CogInitializer& initializer)
{
  // You might grab another component on your object
  // Remember that component could not have Initialize called on it
  // if it were added AFTER your component (see Dependencies)
  mTransform = GetOwner()->has(Transform);
}
</code></pre>
<pre><code class="language-csharp">
void CustomComponent::OnAllObjectsCreated(CogInitializer& initializer)
{
  // Find another object within the space (everything should be created by here)
  Cog* player = GetSpace()->FindObjectByName("Player");
}
</code></pre>
<pre><code class="language-csharp">
void CustomComponent::DebugDraw()
{
  // Draw a red sphere at our position
  gDebugDrawer->Add(Debug::Sphere(mTransform->GetWorldTranslation(), 0.5f).Color(Color::Red));
}
</code></pre>
<pre><code class="language-csharp">
void CustomComponent::OnDestroy(uint flags)
{
  // Disconnect ourselves from any lists we've been added to
}
</code></pre>
Last but not least, if you would like your component to be automatically documented by doxygen, you must use tripple slashes `///` for comments above any classes, functions, properties, or members you want to be documented. The file header that doxygen requires should look something like:

<pre><code class="language-csharp">
*///////////////////////////////////////////////////////////////////////////*
///
/// \file CustomComponent.hpp
/// 
/// Authors: Your Name
///
*///////////////////////////////////////////////////////////////////////////*
</code></pre>

Remember to also put this header in your cpp file and rename `.hpp` to `.cpp`
 

 
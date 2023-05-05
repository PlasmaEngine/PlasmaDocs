# Components

For an introduction what a component is and how it fits into the overall picture, see [The World / Scenegraph System](world-overview.md).

This documentation focuses on the C++ `plComponent` class. The functionality exposed through other mechanisms, such as [TypeScript](../../custom-code/typescript/typescript-overview.md), may be more limited in scope, but ultimately maps to the C++ implementation.

Components are the fundamental building blocks with which to make the engine do things. Components act as glue between systems like the renderer and the user. They expose the available functionality to the editor and they control when and how each system is used. This document describes how components work.

## Owner

A component is always attached to a [game object](game-objects.md). This 'owner' can be queried with `plComponent::GetOwner()`.

There is a brief moment where a component is not attached to an owner, which is when it is being prepared for destruction. If you run into such a situation use `plComponent::IsActiveAndInitialized()` to filter them out.

## Component Manager

Every component has a [component manager](component-managers.md). You can access it with `plComponent::GetOwningManager()`.

To get the component manager for a specific component type, you need to query the [world](worlds.md). See `plWorld::GetOrCreateComponentManager()` and `plWorld::GetOrCreateManagerForComponentType()`.

## Creating Components

The most convenient way to create a component of a specific type is to call the static function `CreateComponent()` on the [component manager](component-managers.md) for that type.

<!-- BEGIN-DOCS-CODE-SNIPPET: create-component -->
```cpp
plMeshComponent* pMesh;
pWorld->GetOrCreateComponentManager<plMeshComponentManager>()->CreateComponent(pObject, pMesh);
```
<!-- END-DOCS-CODE-SNIPPET -->

## Deleting Components

To delete a component, just call `plComponent::DeleteComponent()` on it. Note that deleting individual components is relatively rare, it is more common to just delete the entire object. Also be aware that deleted components are immediately deinitialized. They will still exist in a semi-usable state until the end of the frame, but if other code tries to access the component within the same frame, it may see it in an 'unexpected' state. If necessary, that code can check `plComponent::IsActiveAndInitialized()` to prevent working with just deleted components.

You can also delete a component only through its handle, if you have the corresponding [component manager](component-managers.md).

## Component Handles

When you need to reference components across frames, you should always store *handles* to them, never pointers. See the chapter about [object lifetime](object-lifetime.md) for details.

To convert a handle to a (temporary) pointer, use `plWorld::TryGetComponent()`.

## Querying Components from Game Objects

When you have a [game object](game-objects.md) you can get a list of all attached components with `plGameObject::GetComponents()`. However, typically you want to get a component of a specific type. Use `plGameObject::TryGetComponentOfBaseType()` for that:

<!-- BEGIN-DOCS-CODE-SNIPPET: find-component -->
```cpp
plMeshComponent* pMesh = nullptr;
if (pObject->TryGetComponentOfBaseType(pMesh))
{
  pMesh->DeleteComponent();
}
```
<!-- END-DOCS-CODE-SNIPPET -->

## Iterating over all Components

You can iterate over all components of one type by calling `plComponentManager::GetComponents()`. This returns an iterator with which you can efficiently access all components managed by that component manager. Be aware that some components may not be active, so you should skip those.

You can also access all components on a game object using `plGameObject::GetComponents()`.

## Component Reflection Block

All component types must use [reflection](../reflection-system.md). Only reflected members show up as properties in the editor. An example block looks like this:

<!-- BEGIN-DOCS-CODE-SNIPPET: component-reflection-block -->
```cpp
PLASMA_BEGIN_COMPONENT_TYPE(DebugRenderComponent, 2, plComponentMode::Static)
{
  PLASMA_BEGIN_PROPERTIES
  {
    PLASMA_MEMBER_PROPERTY("Size", m_fSize)->AddAttributes(new plDefaultValueAttribute(1), new plClampValueAttribute(0, 10)),
    PLASMA_MEMBER_PROPERTY("Color", m_Color)->AddAttributes(new plDefaultValueAttribute(plColor::White)),
    PLASMA_ACCESSOR_PROPERTY("Texture", GetTextureFile, SetTextureFile)->AddAttributes(new plAssetBrowserAttribute("Texture 2D")),
    PLASMA_BITFLAGS_MEMBER_PROPERTY("Render", DebugRenderComponentMask, m_RenderTypes)->AddAttributes(new plDefaultValueAttribute(DebugRenderComponentMask::Box)),
  }
  PLASMA_END_PROPERTIES;

  PLASMA_BEGIN_ATTRIBUTES
  {
    new plCategoryAttribute("SampleGamePlugin"), // Component menu group
  }
  PLASMA_END_ATTRIBUTES;

  PLASMA_BEGIN_MESSAGEHANDLERS
  {
    PLASMA_MESSAGE_HANDLER(plMsgSetColor, OnSetColor)
  }
  PLASMA_END_MESSAGEHANDLERS;

  PLASMA_BEGIN_FUNCTIONS
  {
    PLASMA_SCRIPT_FUNCTION_PROPERTY(SetRandomColor)
  }
  PLASMA_END_FUNCTIONS;
}
PLASMA_END_COMPONENT_TYPE
```
<!-- END-DOCS-CODE-SNIPPET -->

The *properties* section lists all the members that should be editable. Components can have 'virtual' properties, that don't exist as members, but use *accessors* (functions). Properties can have *attributes* to configure how they show up in the editor.

The *attributes* section can additionally specify type specific properties. For example, here we tell the editor where in the component menu this component should appear.

The *message handler* section is important to enable [messaging](world-messaging.md).

The *functions* section is used to expose certain member functions to the reflection system, such that script bindings, such as [TypeScript](../../custom-code/typescript/typescript-overview.md) can call these functions.

<!-- TODO: at some point 'we' must document all the available options *sigh* -->

At the moment there is no documentation that lists all the available options. It is best to get inspiration by looking at the code for existing components.

## Component Activation

There are three important states for components:

1. Whether they are **initialized**
1. Whether they are **active**
1. Whether they are **simulating**

You can hook into changes to these states by overriding `plComponent::Initialize()` / `plComponent::Deinitialize()`, `plComponent::OnActivated()` / `plComponent::OnDeactivated()` and `plComponent::OnSimulationStarted()`.

The most important function to override is `plComponent::OnSimulationStarted()`. This is almost always the function where you want to set up your component. It is called when the component is fully initialized, active and the world is actively simulating (the game is running). In the editor, it is only called after you start [running a scene](../../editor/run-scene.md), not while you are editing. Since most game code should not do anything while the scene is being edited, you typically don't need to set up anything before this time.

Components can be 'active' or 'inactive'. This can be used to switch them on and off at will. The [active flag on game objects](game-objects.md#active-flag) affects this, but components can also be deactivated individually with `plComponent::SetActiveFlag()`. When a component is not active, its component manager will typically not update it anymore. If you want to properly support switching components on and off at any time, you often need to be careful to restore state properly. `plComponent::OnActivated()` and `plComponent::OnDeactivated()` will be called every time a component's active state changes. Additionally, if the world is being simulated, `plComponent::OnSimulationStarted()` will also be called after each call to `plComponent::OnActivated()`.

It should be extremely rare that you need to override `plComponent::Initialize()` or `plComponent::Deinitialize()`.

For all the details on the activation functions, refer to the [API Docs](../../api-docs.md).

> **Caution:**
>
> A common mistake is to override a function like `plComponent::OnActivated()` but to not call its base class implementation (`SUPER::OnActivated()`). It is good practice to always do so.

### Forced Activation

If for some reason a component must access another component during its own setup, and requires that other component to be set up first, you can enforce this by calling `plComponent::EnsureSimulationStarted()` on the other component.

An example is a physics joint component. To set up a joint, the component needs to access two rigid body components. Both must be already set up themselves, otherwise the joint component cannot link the two. Therefore, when the joint component is being set up, it  calls `plComponent::EnsureSimulationStarted()` on both rigid body components, to make sure it can access valid data.

## User Flags

`plComponent::SetUserFlag` and `plComponent::GetUserFlag` can be used to store up to 8 bits of user flags. This should only be used internally, to reduce memory consumption.

## Dynamic and Static Components

In the component reflection block you have to specify whether a component is 'dynamic' or 'static':

<!-- BEGIN-DOCS-CODE-SNIPPET: component-reflection -->
```cpp
PLASMA_BEGIN_COMPONENT_TYPE(DemoComponent, 3 /* version */, plComponentMode::Dynamic)
```
<!-- END-DOCS-CODE-SNIPPET -->

This information tells the editor whether this component type attempts to modify the owner's transformation (position, rotation, scale). If any *dynamic* component is attached to a [game object](game-objects.md), the entire object will be marked as dynamic and will have its transform updated every frame. If only *static* components are attached, the game object can be marked as static as well, and costs less performance.

See [Static vs. Dynamic Objects](game-objects.md#static-vs-dynamic-objects).

## Serialization and Versioning

When editing a scene or prefab, the editor will serialize components purely based on reflection information. That means only the properties that are marked up through reflection and are therefore visible to the user are serialized. This format is robust to change (and allows for patches), but is not efficient.

For the runtime format, that a shipping game should use, scenes are *exported*. This is a binary serialization format and every component has full control over what data it writes and how it encodes the data. When you [run a scene](../../editor/run-scene.md) in [plPlayer](../../tools/player.md) the editor will serialize the scene to the binary format, and the player will deserialize it. If a component doesn't properly serialize all its data, the results can range from misconfigured components to crashes during loading.

To implement proper serialization, you need to override `plComponent::SerializeComponent()` and `plComponent::DeserializeComponent()`.

During serialization you simply write data to a stream, as you like:

<!-- BEGIN-DOCS-CODE-SNIPPET: component-serialize -->
```cpp
void DemoComponent::SerializeComponent(plWorldWriter& stream) const
{
  SUPER::SerializeComponent(stream);

  auto& s = stream.GetStream();

  s << m_fAmplitude;
  s << m_Speed;
}
```
<!-- END-DOCS-CODE-SNIPPET -->

Don't forget to call `SUPER::SerializeComponent()` to include the data of the base class.

When you deserialize a component, you need to handle **versioning**. Every component type has a version number, which is specified in the component reflection block:

<!-- BEGIN-DOCS-CODE-SNIPPET: component-reflection -->
```cpp
PLASMA_BEGIN_COMPONENT_TYPE(DemoComponent, 3 /* version */, plComponentMode::Dynamic)
```
<!-- END-DOCS-CODE-SNIPPET -->

The version number should be increased every time the serialization format of the component type has to change. During deserialization you can query the version number with which this component data was written. You than have to handle converting older formats as appropriate:

<!-- BEGIN-DOCS-CODE-SNIPPET: component-deserialize -->
```cpp
void DemoComponent::DeserializeComponent(plWorldReader& stream)
{
  SUPER::DeserializeComponent(stream);
  const plUInt32 uiVersion = stream.GetComponentTypeVersion(GetStaticRTTI());

  auto& s = stream.GetStream();

  s >> m_fAmplitude;

  if (uiVersion <= 2)
  {
    // up to version 2 the angle was stored as a float in degree
    // convert this to plAngle
    float fDegree;
    s >> fDegree;
    m_Speed = plAngle::Degree(fDegree);
  }
  else
  {
    s >> m_Speed;
  }
}
```
<!-- END-DOCS-CODE-SNIPPET -->

## Custom Components

You can extend the engine with custom components:

* [Custom Components with C++](../../custom-code/cpp/custom-cpp-component.md)
* [Custom Components with TypeScript](../../custom-code/typescript/custom-ts-components.md)

## See Also


* [Custom Code](../../custom-code/custom-code-overview.md)
* [The World / Scenegraph System](world-overview.md)
* [Game Objects](game-objects.md)

# Network Serialization

The `plNetworkSerializer` provides automatic, reflection-based property serialization for network components. Properties marked with `plNetSerializeAttribute` are discovered via RTTI, cached per type, and serialized with optional quantization and replication conditions.

## Overview

Instead of writing manual `NetworkSerialize()` / `NetworkDeserialize()` overrides, you can annotate properties in the reflection block and let the serializer handle the rest:

```c++
PL_BEGIN_PROPERTIES
{
  PL_NET_PROPERTY("Health", m_fHealth),
  PL_NET_PROPERTY_HALF("Position", m_vPosition),  // Half-float encoding
  PL_NET_PROPERTY_QUAT("Rotation", m_qRotation),  // Smallest-three encoding
}
PL_END_PROPERTIES;
```

## plNetSerializeAttribute

This attribute marks a property for network serialization. It supports several options:

### Encoding

| Encoding | Description | Use Case |
|----------|-------------|----------|
| `Default` | Full precision (standard Variant serialization) | Most properties |
| `Half` | Half-float (16-bit) for floats and vectors | Positions, velocities |
| `SmallestThree` | Compressed quaternion (smallest 3 components) | Rotations |

### Replication Conditions

Control *when* a property is sent:

| Condition | Description |
|-----------|-------------|
| `Always` | Send every replication tick (default) |
| `OnChange` | Send only when the value differs from the last sent value |
| `InitialOnly` | Send only during initial synchronization (late-joiner) |

### Replication Targets

Control *who* receives a property:

| Target | Description |
|--------|-------------|
| `AllClients` | Send to all clients (default) |
| `OwnerOnly` | Send only to the owning client |
| `NonOwner` | Send to all clients except the owner |

## Helper Macros

The plugin provides convenience macros for common patterns:

| Macro | Encoding | Condition | Target | Visible in Editor |
|-------|----------|-----------|--------|-------------------|
| `PL_NET_PROPERTY(name, member)` | Default | Always | AllClients | No |
| `PL_NET_PROPERTY_HALF(name, member)` | Half | Always | AllClients | No |
| `PL_NET_PROPERTY_QUAT(name, member)` | SmallestThree | Always | AllClients | No |
| `PL_NET_PROPERTY_VISIBLE(name, member)` | Default | Always | AllClients | Yes |
| `PL_NET_PROPERTY_HALF_VISIBLE(name, member)` | Half | Always | AllClients | Yes |
| `PL_NET_PROPERTY_QUAT_VISIBLE(name, member)` | SmallestThree | Always | AllClients | Yes |
| `PL_NET_PROPERTY_INITIAL_ONLY(name, member)` | Default | InitialOnly | AllClients | No |
| `PL_NET_PROPERTY_ON_CHANGE(name, member)` | Default | OnChange | AllClients | No |
| `PL_NET_PROPERTY_OWNER_ONLY(name, member)` | Default | Always | OwnerOnly | No |
| `PL_NET_PROPERTY_NON_OWNER(name, member)` | Default | Always | NonOwner | No |

## Explicit Attribute Construction

For full control, construct the attribute manually:

```c++
PL_MEMBER_PROPERTY("Ammo", m_uiAmmo)
  ->AddAttributes(
    new plNetSerializeAttribute(
      plNetSerializeEncoding::Default,  // encoding
      128,                               // priority (default 128)
      plReplicateCondition::OnChange,    // when to replicate
      plReplicateTarget::OwnerOnly),     // who receives it
    new plHiddenAttribute())
```

## Wire Format

### Basic Format (No Conditions)

Used when a component has no replication conditions:

```
[uint8 propertyCount] [value1] [value2] ... [valueN]
```

All properties are always sent.

### Context-Aware Format (With Conditions)

Used when a component has `OnChange`, `InitialOnly`, `OwnerOnly`, or `NonOwner` properties:

```
[uint32 bitmask] [values for set bits only]
```

Each bit in the bitmask corresponds to a property (in reflection order). Only properties whose bit is set are included in the payload. This reduces bandwidth when using `OnChange` conditions.

## Per-Recipient Serialization

When a component has `OwnerOnly` or `NonOwner` properties, the replication loop performs **per-client serialization**. For each connected client, the serializer evaluates which properties should be included based on whether the client is the owner. This means different clients may receive different subsets of properties.

Components without per-recipient properties are serialized once and broadcast to all clients.

## OnChange Tracking

When `plReplicateCondition::OnChange` is used, the serializer maintains a cache of last-sent values per component. Each tick, it compares the current value against the cached value and only includes the property if it has changed. After sending, the cache is updated.

## Custom Serialization

If automatic serialization does not meet your needs, override `NetworkSerialize()` and `NetworkDeserialize()` on your component:

```c++
void MyComponent::NetworkSerialize(plNetworkMessage& msg) override
{
  // Call base to serialize attributed properties
  plNetworkComponent::NetworkSerialize(msg);

  // Add custom data
  msg.Write<plUInt8>(m_uiCustomField);
}

void MyComponent::NetworkDeserialize(plNetworkMessage& msg) override
{
  plNetworkComponent::NetworkDeserialize(msg);
  m_uiCustomField = msg.Read<plUInt8>();
}
```

## See Also

* [Network Component](network-component.md)
* [Custom Component Tutorial](networking-custom-component.md)

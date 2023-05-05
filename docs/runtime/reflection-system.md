# Reflection System

The Plasma Engine reflection system allows to inspect structs and classes at runtime. It is used primarily for communication with tools and serialization.
The reflection system is macro-based, meaning that it is not generated automatically but needs to be written manually for each type, member, etc that needs to be known at runtime.

## Types

There are four distinct types that can be represented by reflection: classes, structs, enums and bitflags. Each is represented by the `plRTTI` class that stores the type information.

### Classes

Classes are separated into two types: dynamic and static reflected. Dynamic classes derive from `plReflectedClass` which allows you to determine its type using `plReflectedClass::GetDynamicRTTI()`. So with a pointer to an `plReflectedClass` you can access its type information.

A static reflected class does not derive from `plReflectedClass` so it is not possible to get the RTTI information in a common way. However, if you know the type of a variable you can use the template function `plGetStaticRTTI` to retrieve the `plRTTI` instance of a specific type. Alternatively, you can also search for a type by name using `plRTTI::FindTypeByName()`.

```cpp
plReflectedClass* pTest = new plDynamicTestClass;
const plRTTI* pRtti = pTest->GetDynamicRTTI();
const plRTTI* pRtti2 = plGetStaticRTTI<plDynamicTestClass>();
const plRTTI* pRtti3 = plRTTI::FindTypeByName("plDynamicTestClass");
```

Declaring a dynamic class involves deriving from `plReflectedClass`, adding the `PLASMA_ADD_DYNAMIC_REFLECTION(SELF, BASE_TYPE)` macro into the class body and adding a `PLASMA_BEGIN_DYNAMIC_REFLECTED_TYPE(Type, Version, AllocatorType)` block into a compilation unit.

```cpp
//Header
class plDynamicTestClass : public plReflectedClass
{
  PLASMA_ADD_DYNAMIC_REFLECTION(plDynamicTestClass, plReflectedClass);
};
```

```cpp
//Cpp
PLASMA_BEGIN_DYNAMIC_REFLECTED_TYPE(plDynamicTestClass, 1, plRTTIDefaultAllocator<plDynamicTestClass>)
PLASMA_END_DYNAMIC_REFLECTED_TYPE
```

Declaring a static class is very similar to declaring a dynamic class. However, you need to declare the type outside the class via `PLASMA_DECLARE_REFLECTABLE_TYPE(Linkage, TYPE)` and use `PLASMA_BEGIN_STATIC_REFLECTED_TYPE(Type, BaseType, Version, AllocatorType)` in a compilation unit. If a class has no base class, use the dummy class `plNoBase` instead.

```cpp
// Header
class plStaticTestClass
{
};
PLASMA_DECLARE_REFLECTABLE_TYPE(PLASMA_NO_LINKAGE, plStaticTestClass);
```

```cpp
// Cpp
PLASMA_BEGIN_STATIC_REFLECTED_TYPE(plStaticTestClass, plNoBase, 1, plRTTIDefaultAllocator<plStaticTestClass>);
PLASMA_END_STATIC_REFLECTED_TYPE
```

### Structs

Structs are identical to static reflected classes so you can use the exact same macros.

### Enums

Enums are limited to structured enums, i.e. those used by the `plEnum` class. Declaration is similar to static classes, but you use `PLASMA_BEGIN_STATIC_REFLECTED_ENUM(Type, Version)` instead in the compilation unit code.

```cpp
// Header
struct plExampleEnum
{
    typedef plInt8 StorageType;
    enum Enum
    {
    Value1 = 1,          // normal value
    Value2 = -2,         // normal value
    Value3 = 4,          // normal value
    Default = Value1     // Default initialization value (required)
    };
};
PLASMA_DECLARE_REFLECTABLE_TYPE(PLASMA_NO_LINKAGE, plExampleEnum);
```

```cpp
// Cpp
PLASMA_BEGIN_STATIC_REFLECTED_ENUM(plExampleEnum, 1)
  PLASMA_ENUM_CONSTANTS(plExampleEnum::Value1, plExampleEnum::Value2)
  PLASMA_ENUM_CONSTANT(plExampleEnum::Value3),
PLASMA_END_STATIC_REFLECTED_ENUM
```

The enum constants can either be declared via `PLASMA_ENUM_CONSTANTS()` or `PLASMA_ENUM_CONSTANT(Value)` inside the begin / end block of the enum declaration. An enum type can be identified by its base type which is always the dummy `plEnumBase`.

### Bitflags

Bitflags are limited to structured bitflags, i.e. those used by the `plBitflags` class. Declaration is similar to static classes, but you use `PLASMA_BEGIN_STATIC_REFLECTED_BITFLAGS(Type, Version)` instead in the compilation unit code.

```cpp
// Header
struct plExampleBitflags
{
    typedef plUInt64 StorageType;
    enum Enum : plUInt64
    {
    Value1 = PLASMA_BIT(0),  // normal value
    Value2 = PLASMA_BIT(31), // normal value
    Value3 = PLASMA_BIT(63), // normal value
    Default = Value1     // Default initialization value (required)
    };

    struct Bits
    {
    StorageType Value1 : 1;
    StorageType Padding : 30;
    StorageType Value2 : 1;
    StorageType Padding2 : 31;
    StorageType Value3 : 1;
    };
};
PLASMA_DECLARE_REFLECTABLE_TYPE(PLASMA_NO_LINKAGE, plExampleBitflags);
```

```cpp
// Cpp
PLASMA_BEGIN_STATIC_REFLECTED_BITFLAGS(plExampleBitflags, 1)
  PLASMA_BITFLAGS_CONSTANTS(plExampleBitflags::Value1, plExampleBitflags::Value2)
  PLASMA_BITFLAGS_CONSTANT(plExampleBitflags::Value3),
PLASMA_END_STATIC_REFLECTED_BITFLAGS();
```

The bitflags constants can either be declared via `PLASMA_BITFLAGS_CONSTANTS()` or `PLASMA_BITFLAGS_CONSTANT(Value)` inside the begin / end block of the bitflags declaration. A bitflags type can be identified by its base type which is always the dummy `plBitflagsBase`.
  
## Properties

Properties are the most important information in a type as they define the data inside it. The properties of a type can be accessed via `plRTTI::GetProperties()`. There are different categories of properties, each deriving from `plAbstractProperty`. The type of property can be determined by calling `plAbstractProperty::GetCategory()`.
Properties are added via the property macros inside the `PLASMA_BEGIN_PROPERTIES()` / `PLASMA_END_PROPERTIES()` block of the type declaration like this:

```cpp
PLASMA_BEGIN_STATIC_REFLECTED_TYPE(plStaticTestClass, plNoBase, 1, plRTTIDefaultAllocator<plStaticTestClass>)
{
    PLASMA_BEGIN_PROPERTIES
    {
        PLASMA_CONSTANT_PROPERTY("Constant", 5),
        PLASMA_MEMBER_PROPERTY("Member", m_fFloat),
        PLASMA_ACCESSOR_PROPERTY("MemberAccessor", GetInt, SetInt),
        PLASMA_ARRAY_MEMBER_PROPERTY("Array", m_Deque),
        PLASMA_ARRAY_ACCESSOR_PROPERTY("ArrayAccessor", GetCount, GetValue, SetValue, Insert, Remove),
        PLASMA_SET_MEMBER_PROPERTY("Set", m_SetMember),
        PLASMA_SET_ACCESSOR_PROPERTY("SetAccessor", GetSet, SetInsert, SetRemove),
    }
    PLASMA_END_PROPERTIES
}
PLASMA_END_STATIC_REFLECTED_TYPE();
```

### Constants

Constants are declared via `PLASMA_CONSTANT_PROPERTY(PropertyName, Value)`. The value is stored within the property so no instance of the class is necessary to access it. To access the constant, cast the property to `plAbstractConstantProperty` and call `plAbstractConstantProperty::GetPropertyType()` to determine the constant type. Then either cast to `plTypedConstantProperty` of the matching type, or if the type is not known to you at compile time, use `plAbstractConstantProperty::GetPropertyPointer()` to access its data.

### Members

There are two types of member properties, direct member properties and accessor properties. The first has direct access to the memory location of the property in the class while the later uses functions to get and set the property's value.
Direct member properties are declared via `PLASMA_MEMBER_PROPERTY(PropertyName, MemberName)` while accessor properties are declared via `PLASMA_ACCESSOR_PROPERTY(PropertyName, Getter, Setter)`. The getter and setter functions must have the following signature:

```cpp
Type GetterFunc() const;
void SetterFunc(Type value);
```

Type can be decorated with const and reference but must be consistent between get and set function. The available macros are the following:

```cpp
PLASMA_MEMBER_PROPERTY("Member", m_fFloat1),
PLASMA_MEMBER_PROPERTY_READ_ONLY("MemberRO", m_vProperty3),
PLASMA_ACCESSOR_PROPERTY("MemberAccessor", GetInt, SetInt),
PLASMA_ACCESSOR_PROPERTY_READ_ONLY("MemberAccessorRO", GetInt),
```

To access an instance's member variable value, cast the property to `plAbstractMemberProperty` and call `plAbstractMemberProperty::GetPropertyType()` to determine the member type. Then either cast to `plTypedMemberProperty` of the matching type, or if the type is not known to you at compile time, use `plAbstractMemberProperty::GetPropertyPointer()` or `plAbstractMemberProperty::GetValuePtr()` and `plAbstractMemberProperty::SetValuePtr()` to access its data. The first solution will only return a valid pointer if the property is a direct member property.

### Arrays

Array properties are very similar to member properties, they just handle arrays instead of single values. Direct array properties are declared via `PLASMA_ARRAY_MEMBER_PROPERTY(PropertyName, MemberName)` while accessor array properties are declared via `PLASMA_ARRAY_ACCESSOR_PROPERTY(PropertyName, GetCount, Getter, Setter, Insert, Remove)`. The accessor interface functions must have the following signature:

```cpp
plUInt32 GetCount() const;
Type GetValue(plUInt32 uiIndex) const;
void SetValue(plUInt32 uiIndex, Type value);
void Insert(plUInt32 uiIndex, Type value);
void Remove(plUInt32 uiIndex);
```

The available macros are the following:

```cpp
PLASMA_ARRAY_ACCESSOR_PROPERTY("ArrayAccessor", GetCount, GetValue, SetValue, Insert, Remove),
PLASMA_ARRAY_ACCESSOR_PROPERTY_READ_ONLY("ArrayAccessorRO", GetCount, GetValue),
PLASMA_ARRAY_MEMBER_PROPERTY("Hybrid", m_Hybrid),
PLASMA_ARRAY_MEMBER_PROPERTY("Dynamic", m_Dynamic),
PLASMA_ARRAY_MEMBER_PROPERTY_READ_ONLY("Deque", m_Deque),
```

To access an instance's array, cast the property to `plAbstractArrayProperty` and call `plAbstractArrayProperty::GetElementType()` to determine the element type. From here you can use the various functions inside `plAbstractArrayProperty` to manipulate an instance's array.

### Sets

Set properties are very similar to member properties, they just handle sets instead of single values. Direct set properties are declared via `PLASMA_SET_MEMBER_PROPERTY(PropertyName, MemberName)` while accessor set properties are declared via `PLASMA_SET_ACCESSOR_PROPERTY(PropertyName, GetValues, Insert, Remove)`. The accessor interface functions must have the following signature:

```cpp
void Insert(Type value);
void Remove(Type value);
Container<Type> GetValues() const;
```

The available macros are the following:  

```cpp
PLASMA_SET_ACCESSOR_PROPERTY("SetAccessor", GetValues, Insert, Remove),
PLASMA_SET_ACCESSOR_PROPERTY_READ_ONLY("SetAccessorRO", GetValues),
PLASMA_SET_MEMBER_PROPERTY("Set", m_SetMember),
PLASMA_SET_MEMBER_PROPERTY_READ_ONLY("SetRO", m_SetMember),
```

To access an instance's set, cast the property to `plAbstractSetProperty` and call `plAbstractSetProperty::GetElementType()` to determine the element type. From here you can use the various functions inside `plAbstractSetProperty` to manipulate an instance's set.

## Flags

Types as well as properties have flags that quickly let you determine the kind of type / property you are dealing with.
For types, `plRTTI::GetTypeFlags()` lets you access its `plTypeFlags::Enum` flags which are automatically deduced from the type at compile time.

Properties can have flags as well, `plAbstractMemberProperty::GetFlags()`, `plAbstractArrayProperty::GetFlags()` and `plAbstractSetProperty::GetFlags()` let you access the `plPropertyFlags::Enum` flags of the handled property type. The only difference here is that besides automatically deduced flags there are also user-defined flags that can be added during declaration of the property by using `plAbstractMemberProperty::AddFlags` and the variants on the other property categories:

```cpp
PLASMA_ACCESSOR_PROPERTY("ArraysPtr", GetArrays, SetArrays)->AddFlags(plPropertyFlags::PointerOwner),
```

## Limitations

* No two types can share the same name.
* Each property name must be unique within its type.
* Only constants that are a basic type (i.e. can be stored inside an `plVariant`) will be available to tools.
* A pointer to a type cannot be its own type, the only exception to this is const char*.



 `Component` `Engine`



(NOTE) Transform component class. The transform component provides the position, rotation and scale of an object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RotateAnglesLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotateangleslocal-void)|[ EulerAngles](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#eulerangles-plasma-engine)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ RotateAnglesWorld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotateanglesworld-void)|[ LocalRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#localrotation-plasma-engin)| | |
|[ RotateAround](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotatearound-void)|[ LocalScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#localscale-plasma-engine-d)| | |
|[ RotateLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotatelocal-void)|[ LocalTranslation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#localtranslation-plasma-en)| | |
|[ RotateWorld](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotateworld-void)|[ Parent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#parent-plasma-engine-docum)| | |
|[ SetEulerAnglesXYZ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#seteuleranglesxyz-void)|[ Rotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#rotation-plasma-engine-doc)| | |
|[ SetRotationBases](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#setrotationbases-void)|[ Scale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#scale-plasma-engine-docume)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transform-void)|[ Translation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#translation-plasma-engine)| | |
|[ TransformNormal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformnormal-plasma-eng)|[ WorldMatrix](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#worldmatrix-plasma-engine)| | |
|[ TransformNormalInverse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformnormalinverse-z)|[ WorldRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#worldrotation-plasma-engin)| | |
|[ TransformNormalLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformnormallocal-zer)|[ WorldScale](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#worldscale-plasma-engine-d)| | |
|[ TransformPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformpoint-plasma-engi)|[ WorldTranslation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#worldtranslation-plasma-en)| | |
|[ TransformPointInverse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformpointinverse-ze)| | | |
|[ TransformPointLocal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md#transformpointlocal-plasma)| | | |


 #  Properties


---  
 #  EulerAngles : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The rotation of the transform as an Euler angle vector in radians.
> ``` lang=cpp, name=Lightning
> var EulerAngles : Real3


---  
 #  LocalRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Local rotation relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalRotation : Quaternion


---  
 #  LocalScale : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Local Scale relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalScale : Real3


---  
 #  LocalTranslation : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Local Translation relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalTranslation : Real3


---  
 #  Parent : [transform](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/transform.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Parent : Transform


---  
 #  Rotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Local rotation relative to parent.
> ``` lang=cpp, name=Lightning
> var Rotation : Quaternion


---  
 #  Scale : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Local Scale relative to parent.
> ``` lang=cpp, name=Lightning
> var Scale : Real3


---  
 #  Translation : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Local Translation relative to parent.
> ``` lang=cpp, name=Lightning
> var Translation : Real3


---  
 #  WorldMatrix : [real4x4](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real4x4.md)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var WorldMatrix : Real4x4


---  
 #  WorldRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Rotation in World Space.
> ``` lang=cpp, name=Lightning
> var WorldRotation : Quaternion


---  
 #  WorldScale : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Scale in World Space.
> ``` lang=cpp, name=Lightning
> var WorldScale : Real3


---  
 #  WorldTranslation : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Translation in World Space.
> ``` lang=cpp, name=Lightning
> var WorldTranslation : Real3


---  
 #  Methods


---  
 #  RotateAnglesLocal : Void

> Rotate object in local space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function RotateAnglesLocal(angles : Real3)
> ``` 


---  
 #  RotateAnglesWorld : Void

> Rotate object in world space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function RotateAnglesWorld(angles : Real3)
> ``` 


---  
 #  RotateAround : Void

> Rotate around a given point with the given rotation.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |rotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)| |
> ``` lang=cpp, name=Lightning
> function RotateAround(point : Real3, rotation : Quaternion)
> ``` 


---  
 #  RotateLocal : Void

> Rotate object in local space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)| |
> ``` lang=cpp, name=Lightning
> function RotateLocal(rotation : Quaternion)
> ``` 


---  
 #  RotateWorld : Void

> Rotate object in world space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)| |
> ``` lang=cpp, name=Lightning
> function RotateWorld(rotation : Quaternion)
> ``` 


---  
 #  SetEulerAnglesXYZ : Void

> Sets the rotation of the transform by the given Euler angles in radians.
> |Name|Type|Description|
> |---|---|---|
> |xRadians|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |yRadians|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> |zRadians|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)| |
> ``` lang=cpp, name=Lightning
> function SetEulerAnglesXYZ(xRadians : Real, yRadians : Real, zRadians : Real)
> ``` 


---  
 #  SetRotationBases : Void

> Generates a rotation matrix from the given bases.
> |Name|Type|Description|
> |---|---|---|
> |facing|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |right|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function SetRotationBases(facing : Real3, up : Real3, right : Real3)
> ``` 


---  
 #  Transform : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Transform()
> ``` 


---  
 #  TransformNormal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a local normal (direction) into world space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformNormal(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalInverse : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a world normal (direction) into local space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformNormalInverse(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalLocal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a normal by the local matrix (ignores parent's transform) Needed now because there is no quaternion times vector in script.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformNormalLocal(normal : Real3) : Real3
> ``` 


---  
 #  TransformPoint : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a local point into world space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformPoint(point : Real3) : Real3
> ``` 


---  
 #  TransformPointInverse : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a world point into local space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformPointInverse(point : Real3) : Real3
> ``` 


---  
 #  TransformPointLocal : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> Transforms a point by the local matrix (ignores parent's transform)
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function TransformPointLocal(point : Real3) : Real3
> ``` 


---  
 

 
 `Component` `Engine`



(NOTE) Transform component class. The transform component provides the position, rotation and scale of an object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RotateAnglesLocal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotateangleslocal-void)|[ EulerAngles](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#eulerangles-plasma-engine)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ RotateAnglesWorld](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotateanglesworld-void)|[ LocalRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#localrotation-plasma-engin)| | |
|[ RotateAround](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotatearound-void)|[ LocalScale](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#localscale-plasma-engine-d)| | |
|[ RotateLocal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotatelocal-void)|[ LocalTranslation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#localtranslation-plasma-en)| | |
|[ RotateWorld](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotateworld-void)|[ Parent](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#parent-plasma-engine-docum)| | |
|[ SetEulerAnglesXYZ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#seteuleranglesxyz-void)|[ Rotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#rotation-plasma-engine-doc)| | |
|[ SetRotationBases](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#setrotationbases-void)|[ Scale](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#scale-plasma-engine-docume)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transform-void)|[ Translation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#translation-plasma-engine)| | |
|[ TransformNormal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformnormal-plasma-eng)|[ WorldMatrix](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#worldmatrix-plasma-engine)| | |
|[ TransformNormalInverse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformnormalinverse-z)|[ WorldRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#worldrotation-plasma-engin)| | |
|[ TransformNormalLocal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformnormallocal-zer)|[ WorldScale](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#worldscale-plasma-engine-d)| | |
|[ TransformPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformpoint-plasma-engi)|[ WorldTranslation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#worldtranslation-plasma-en)| | |
|[ TransformPointInverse](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformpointinverse-ze)| | | |
|[ TransformPointLocal](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown#transformpointlocal-plasma)| | | |


 #  Properties


---  
 #  EulerAngles : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The rotation of the transform as an Euler angle vector in radians.
> ``` lang=cpp, name=Lightning
> var EulerAngles : Real3


---  
 #  LocalRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Local rotation relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalRotation : Quaternion


---  
 #  LocalScale : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Local Scale relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalScale : Real3


---  
 #  LocalTranslation : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Local Translation relative to parent.
> ``` lang=cpp, name=Lightning
> var LocalTranslation : Real3


---  
 #  Parent : [transform](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/transform.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var Parent : Transform


---  
 #  Rotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Local rotation relative to parent.
> ``` lang=cpp, name=Lightning
> var Rotation : Quaternion


---  
 #  Scale : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Local Scale relative to parent.
> ``` lang=cpp, name=Lightning
> var Scale : Real3


---  
 #  Translation : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Local Translation relative to parent.
> ``` lang=cpp, name=Lightning
> var Translation : Real3


---  
 #  WorldMatrix : [real4x4](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real4x4.markdown)

 `read-only`

> 
> ``` lang=cpp, name=Lightning
> var WorldMatrix : Real4x4


---  
 #  WorldRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Rotation in World Space.
> ``` lang=cpp, name=Lightning
> var WorldRotation : Quaternion


---  
 #  WorldScale : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Scale in World Space.
> ``` lang=cpp, name=Lightning
> var WorldScale : Real3


---  
 #  WorldTranslation : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

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
> |angles|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function RotateAnglesLocal(angles : Real3)
> ``` 


---  
 #  RotateAnglesWorld : Void

> Rotate object in world space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function RotateAnglesWorld(angles : Real3)
> ``` 


---  
 #  RotateAround : Void

> Rotate around a given point with the given rotation.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |rotation|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function RotateAround(point : Real3, rotation : Quaternion)
> ``` 


---  
 #  RotateLocal : Void

> Rotate object in local space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function RotateLocal(rotation : Quaternion)
> ``` 


---  
 #  RotateWorld : Void

> Rotate object in world space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function RotateWorld(rotation : Quaternion)
> ``` 


---  
 #  SetEulerAnglesXYZ : Void

> Sets the rotation of the transform by the given Euler angles in radians.
> |Name|Type|Description|
> |---|---|---|
> |xRadians|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |yRadians|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> |zRadians|[real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetEulerAnglesXYZ(xRadians : Real, yRadians : Real, zRadians : Real)
> ``` 


---  
 #  SetRotationBases : Void

> Generates a rotation matrix from the given bases.
> |Name|Type|Description|
> |---|---|---|
> |facing|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |right|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
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
 #  TransformNormal : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a local normal (direction) into world space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformNormal(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalInverse : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a world normal (direction) into local space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformNormalInverse(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalLocal : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a normal by the local matrix (ignores parent's transform) Needed now because there is no quaternion times vector in script.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformNormalLocal(normal : Real3) : Real3
> ``` 


---  
 #  TransformPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a local point into world space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformPoint(point : Real3) : Real3
> ``` 


---  
 #  TransformPointInverse : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a world point into local space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformPointInverse(point : Real3) : Real3
> ``` 


---  
 #  TransformPointLocal : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> Transforms a point by the local matrix (ignores parent's transform)
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function TransformPointLocal(point : Real3) : Real3
> ``` 


---  
 

 
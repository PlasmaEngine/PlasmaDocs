 `Component` `Gameplay`



(NOTE) Defines a new basis for a desired right, up, and forward vector. Provides a bunch of helper functions to change between these spaces and to perform simple look-at behavior.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeSignedAngle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#computesignedangle-plasma)|[ AbsoluteAngle](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#absoluteangle-plasma-engin)|[component](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/component.md)| |
|[ DebugDrawBases](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#debugdrawbases-void)|[ DefaultOrientationBases](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#defaultorientationbases)| | |
|[ GetLookAtDirectionRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#getlookatdirectionrotati)|[ GlobalUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#globalup-plasma-engine-doc)| | |
|[ GetLookAtDirectionWithUpRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#getlookatdirectionwithup)|[ LocalForward](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localforward-plasma-engine)| | |
|[ GetLookAtPointRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#getlookatpointrotation-z)|[ LocalOrientationBasis](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localorientationbasis-ze)| | |
|[ GetLookAtPointWithUpRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#getlookatpointwithuprota)|[ LocalRight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localright-plasma-engine-d)| | |
|[ LookAtDirection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#lookatdirection-void)|[ LocalToOrientationRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localtoorientationrotati)| | |
|[ LookAtDirectionWithUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#lookatdirectionwithup-vo)|[ LocalToWorldRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localtoworldrotation-zer)| | |
|[ LookAtPoint](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#lookatpoint-void)|[ LocalUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#localup-plasma-engine-docu)| | |
|[ LookAtPointWithUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#lookatpointwithup-void)|[ OrientationForward](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientationforward-plasma)| | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientation-void)|[ OrientationRight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientationright-plasma-en)| | |
|[ SetLocalLookAtRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#setlocallookatrotation-v)|[ OrientationToLocalRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientationtolocalrotati)| | |
|[ SetWorldLookAtRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#setworldlookatrotation-v)|[ OrientationToWorldRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientationtoworldrotati)| | |
| |[ OrientationUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#orientationup-plasma-engin)| | |
| |[ WorldForward](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#worldforward-plasma-engine)| | |
| |[ WorldRight](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#worldright-plasma-engine-d)| | |
| |[ WorldToLocalRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#worldtolocalrotation-zer)| | |
| |[ WorldToOrientationRotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#worldtoorientationrotati)| | |
| |[ WorldUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/orientation.md#worldup-plasma-engine-docu)| | |


 #  Properties


---  
 #  AbsoluteAngle : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

 `read-only`

> Get the angle of the object about the up vector.
> ``` lang=cpp, name=Lightning
> var AbsoluteAngle : Real


---  
 #  DefaultOrientationBases : [OrientationBases](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#orientationbases)

> 
> ``` lang=cpp, name=Lightning
> var DefaultOrientationBases : OrientationBases


---  
 #  GlobalUp : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

> The world-space up vector to use for LookAt operations that don't take an up vector.
> ``` lang=cpp, name=Lightning
> var GlobalUp : Real3


---  
 #  LocalForward : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalForward : Real3


---  
 #  LocalOrientationBasis : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> A local-space basis that represents this orientation. If you build a basis from an up of (0, 1, 0), and a forward of (0, 0, -1) then this should result in the identity rotation.
> ``` lang=cpp, name=Lightning
> var LocalOrientationBasis : Quaternion


---  
 #  LocalRight : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalRight : Real3


---  
 #  LocalToOrientationRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that takes an local space vector into orientation space. For example, this transforms LocalRight into OrientationRight.
> ``` lang=cpp, name=Lightning
> var LocalToOrientationRotation : Quaternion


---  
 #  LocalToWorldRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from local space into world space. For example, this transforms LocalRight into WorldRight.
> ``` lang=cpp, name=Lightning
> var LocalToWorldRotation : Quaternion


---  
 #  LocalUp : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalUp : Real3


---  
 #  OrientationForward : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The forward vector in orientation space. This is always the vector (0, 0, -1) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationForward : Real3


---  
 #  OrientationRight : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The right vector in orientation space. This is always the vector (1, 0, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationRight : Real3


---  
 #  OrientationToLocalRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into local space. For example, this transforms OrientationRight into LocalRight.
> ``` lang=cpp, name=Lightning
> var OrientationToLocalRotation : Quaternion


---  
 #  OrientationToWorldRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into world space. For example, this transforms OrientationRight into WorldRight.
> ``` lang=cpp, name=Lightning
> var OrientationToWorldRotation : Quaternion


---  
 #  OrientationUp : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The up vector in orientation space. This is always the vector (0, 1, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationUp : Real3


---  
 #  WorldForward : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldForward : Real3


---  
 #  WorldRight : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldRight : Real3


---  
 #  WorldToLocalRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from world space into local space. For example, this transforms WorldRight into LocalRight.
> ``` lang=cpp, name=Lightning
> var WorldToLocalRotation : Quaternion


---  
 #  WorldToOrientationRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

 `read-only`

> The rotation that takes an world space vector into orientation space. For example, this transforms WorldRight into OrientationRight.
> ``` lang=cpp, name=Lightning
> var WorldToOrientationRotation : Quaternion


---  
 #  WorldUp : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldUp : Real3


---  
 #  Methods


---  
 #  ComputeSignedAngle : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> Compute the rotation angle between two vectors (in radians)
> |Name|Type|Description|
> |---|---|---|
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |forward|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |newVector|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function ComputeSignedAngle(up : Real3, forward : Real3, newVector : Real3) : Real
> ``` 


---  
 #  DebugDrawBases : Void

> Debug draws the current orientation bases in world space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DebugDrawBases()
> ``` 


---  
 #  GetLookAtDirectionRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Gets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtDirectionRotation(lookDir : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtDirectionWithUpRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Same as GetLookAtDirectionRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtDirectionWithUpRotation(lookDir : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Get the rotation so that the forward will look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtPointRotation(lookPoint : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointWithUpRotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)

> Same as GetLookAtPointRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtPointWithUpRotation(lookPoint : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  LookAtDirection : Void

> Sets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function LookAtDirection(lookDir : Real3)
> ``` 


---  
 #  LookAtDirectionWithUp : Void

> Same as LookAtDirection but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function LookAtDirectionWithUp(lookDir : Real3, up : Real3)
> ``` 


---  
 #  LookAtPoint : Void

> Sets the forward to look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function LookAtPoint(lookPoint : Real3)
> ``` 


---  
 #  LookAtPointWithUp : Void

> Same as LookAtPoint but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> |up|[real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.md)| |
> ``` lang=cpp, name=Lightning
> function LookAtPointWithUp(lookPoint : Real3, up : Real3)
> ``` 


---  
 #  Orientation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Orientation()
> ``` 


---  
 #  SetLocalLookAtRotation : Void

> Set the transform's local rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |localLookAtRotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)| |
> ``` lang=cpp, name=Lightning
> function SetLocalLookAtRotation(localLookAtRotation : Quaternion)
> ``` 


---  
 #  SetWorldLookAtRotation : Void

> Set the transform's world rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |worldLookAtRotation|[quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.md)| |
> ``` lang=cpp, name=Lightning
> function SetWorldLookAtRotation(worldLookAtRotation : Quaternion)
> ``` 


---  
 

 
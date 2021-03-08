 `Component` `Gameplay`



(NOTE) Defines a new basis for a desired right, up, and forward vector. Provides a bunch of helper functions to change between these spaces and to perform simple look-at behavior.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeSignedAngle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#computesignedangle-plasma)|[ AbsoluteAngle](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#absoluteangle-plasma-engin)|[component](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/component.markdown)| |
|[ DebugDrawBases](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#debugdrawbases-void)|[ DefaultOrientationBases](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#defaultorientationbases)| | |
|[ GetLookAtDirectionRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#getlookatdirectionrotati)|[ GlobalUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#globalup-plasma-engine-doc)| | |
|[ GetLookAtDirectionWithUpRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#getlookatdirectionwithup)|[ LocalForward](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localforward-plasma-engine)| | |
|[ GetLookAtPointRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#getlookatpointrotation-z)|[ LocalOrientationBasis](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localorientationbasis-ze)| | |
|[ GetLookAtPointWithUpRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#getlookatpointwithuprota)|[ LocalRight](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localright-plasma-engine-d)| | |
|[ LookAtDirection](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#lookatdirection-void)|[ LocalToOrientationRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localtoorientationrotati)| | |
|[ LookAtDirectionWithUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#lookatdirectionwithup-vo)|[ LocalToWorldRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localtoworldrotation-zer)| | |
|[ LookAtPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#lookatpoint-void)|[ LocalUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#localup-plasma-engine-docu)| | |
|[ LookAtPointWithUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#lookatpointwithup-void)|[ OrientationForward](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientationforward-plasma)| | |
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientation-void)|[ OrientationRight](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientationright-plasma-en)| | |
|[ SetLocalLookAtRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#setlocallookatrotation-v)|[ OrientationToLocalRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientationtolocalrotati)| | |
|[ SetWorldLookAtRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#setworldlookatrotation-v)|[ OrientationToWorldRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientationtoworldrotati)| | |
| |[ OrientationUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#orientationup-plasma-engin)| | |
| |[ WorldForward](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#worldforward-plasma-engine)| | |
| |[ WorldRight](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#worldright-plasma-engine-d)| | |
| |[ WorldToLocalRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#worldtolocalrotation-zer)| | |
| |[ WorldToOrientationRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#worldtoorientationrotati)| | |
| |[ WorldUp](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/orientation.markdown#worldup-plasma-engine-docu)| | |


 #  Properties


---  
 #  AbsoluteAngle : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

 `read-only`

> Get the angle of the object about the up vector.
> ``` lang=cpp, name=Lightning
> var AbsoluteAngle : Real


---  
 #  DefaultOrientationBases : [OrientationBases](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/enum_reference.markdown#orientationbases)

> 
> ``` lang=cpp, name=Lightning
> var DefaultOrientationBases : OrientationBases


---  
 #  GlobalUp : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The world-space up vector to use for LookAt operations that don't take an up vector.
> ``` lang=cpp, name=Lightning
> var GlobalUp : Real3


---  
 #  LocalForward : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's forward vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalForward : Real3


---  
 #  LocalOrientationBasis : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> A local-space basis that represents this orientation. If you build a basis from an up of (0, 1, 0), and a forward of (0, 0, -1) then this should result in the identity rotation.
> ``` lang=cpp, name=Lightning
> var LocalOrientationBasis : Quaternion


---  
 #  LocalRight : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's right vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalRight : Real3


---  
 #  LocalToOrientationRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that takes an local space vector into orientation space. For example, this transforms LocalRight into OrientationRight.
> ``` lang=cpp, name=Lightning
> var LocalToOrientationRotation : Quaternion


---  
 #  LocalToWorldRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that transforms a vector from local space into world space. For example, this transforms LocalRight into WorldRight.
> ``` lang=cpp, name=Lightning
> var LocalToWorldRotation : Quaternion


---  
 #  LocalUp : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's up vector after having been transformed into local space.
> ``` lang=cpp, name=Lightning
> var LocalUp : Real3


---  
 #  OrientationForward : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The forward vector in orientation space. This is always the vector (0, 0, -1) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationForward : Real3


---  
 #  OrientationRight : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The right vector in orientation space. This is always the vector (1, 0, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationRight : Real3


---  
 #  OrientationToLocalRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that takes an orientation space vector into local space. For example, this transforms OrientationRight into LocalRight.
> ``` lang=cpp, name=Lightning
> var OrientationToLocalRotation : Quaternion


---  
 #  OrientationToWorldRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that takes an orientation space vector into world space. For example, this transforms OrientationRight into WorldRight.
> ``` lang=cpp, name=Lightning
> var OrientationToWorldRotation : Quaternion


---  
 #  OrientationUp : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The up vector in orientation space. This is always the vector (0, 1, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Lightning
> var OrientationUp : Real3


---  
 #  WorldForward : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's forward vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldForward : Real3


---  
 #  WorldRight : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's right vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldRight : Real3


---  
 #  WorldToLocalRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that transforms a vector from world space into local space. For example, this transforms WorldRight into LocalRight.
> ``` lang=cpp, name=Lightning
> var WorldToLocalRotation : Quaternion


---  
 #  WorldToOrientationRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

 `read-only`

> The rotation that takes an world space vector into orientation space. For example, this transforms WorldRight into OrientationRight.
> ``` lang=cpp, name=Lightning
> var WorldToOrientationRotation : Quaternion


---  
 #  WorldUp : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

 `read-only`

> The orientation's up vector after having been transformed into world space.
> ``` lang=cpp, name=Lightning
> var WorldUp : Real3


---  
 #  Methods


---  
 #  ComputeSignedAngle : [real](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real.markdown)

> Compute the rotation angle between two vectors (in radians)
> |Name|Type|Description|
> |---|---|---|
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |forward|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |newVector|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
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
 #  GetLookAtDirectionRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Gets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtDirectionRotation(lookDir : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtDirectionWithUpRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Same as GetLookAtDirectionRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtDirectionWithUpRotation(lookDir : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Get the rotation so that the forward will look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtPointRotation(lookPoint : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointWithUpRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Same as GetLookAtPointRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function GetLookAtPointWithUpRotation(lookPoint : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  LookAtDirection : Void

> Sets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function LookAtDirection(lookDir : Real3)
> ``` 


---  
 #  LookAtDirectionWithUp : Void

> Same as LookAtDirection but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function LookAtDirectionWithUp(lookDir : Real3, up : Real3)
> ``` 


---  
 #  LookAtPoint : Void

> Sets the forward to look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> ``` lang=cpp, name=Lightning
> function LookAtPoint(lookPoint : Real3)
> ``` 


---  
 #  LookAtPointWithUp : Void

> Same as LookAtPoint but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
> |up|[real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)| |
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
> |localLookAtRotation|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetLocalLookAtRotation(localLookAtRotation : Quaternion)
> ``` 


---  
 #  SetWorldLookAtRotation : Void

> Set the transform's world rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |worldLookAtRotation|[quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)| |
> ``` lang=cpp, name=Lightning
> function SetWorldLookAtRotation(worldLookAtRotation : Quaternion)
> ``` 


---  
 

 
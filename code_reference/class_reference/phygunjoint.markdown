 `Component` `Physics`



(NOTE) Legacy. A physics gun joint is an experimental joint for picking up objects. This acts as a weld between an object and the world. Primarily an experiment for picking up objects as a player. Should be custom implemented in script with CustomJoint instead.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#phygunjoint-void)|[ LocalPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#localpoint-plasma-engine-d)|[joint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/joint.markdown)| |
| |[ TargetPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#targetpoint-plasma-engine)| | |
| |[ TargetRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#targetrotation-plasma-engi)| | |
| |[ WorldPoint](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#worldpoint-plasma-engine-d)| | |
| |[ WorldRotation](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/phygunjoint.markdown#worldrotation-plasma-engin)| | |


 #  Properties


---  
 #  LocalPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The local point on the object that should match the target point.
> ``` lang=cpp, name=Lightning
> var LocalPoint : Real3


---  
 #  TargetPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The point in world space that the object's point should match.
> ``` lang=cpp, name=Lightning
> var TargetPoint : Real3


---  
 #  TargetRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> The world space rotation that the basis of the object should match. Used to set the desired rotation of the object in world space.
> ``` lang=cpp, name=Lightning
> var TargetRotation : Quaternion


---  
 #  WorldPoint : [real3](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/real3.markdown)

> The world point on the object that should match the target point.
> ``` lang=cpp, name=Lightning
> var WorldPoint : Real3


---  
 #  WorldRotation : [quaternion](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/lightning_base_types/quaternion.markdown)

> Used to set the world rotation basis of the object that should be matched to the target rotation.
> ``` lang=cpp, name=Lightning
> var WorldRotation : Quaternion


---  
 #  Methods


---  
 #  PhyGunJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function PhyGunJoint()
> ``` 


---  
 

 
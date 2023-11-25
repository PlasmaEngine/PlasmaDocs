 `Physics`

(NOTE) A block of information for solving a joint (or constraint) type. This is used to configure how one joint is solved independently of another joint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AngularBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#angularbaumgarte-plasma-en)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.md)|[contactblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactblock.md)|
| |[ AngularErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#angularerrorcorrection-z)| |[customjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointblock.md)|
| |[ LinearBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#linearbaumgarte-plasma-eng)| |[fixedanglejointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/fixedanglejointblock.md)|
| |[ LinearErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#linearerrorcorrection-ze)| |[gearjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjointblock.md)|
| |[ PositionCorrectionType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#positioncorrectiontype-z)| |[linearaxisjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearaxisjointblock.md)|
| |[ Slop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.md#slop-plasma-engine-documen)| |[manipulatorjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjointblock.md)|
| | | |[phygunjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/phygunjointblock.md)|
| | | |[positionjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjointblock.md)|
| | | |[prismaticjoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2dblock.md)|
| | | |[prismaticjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjointblock.md)|
| | | |[pulleyjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjointblock.md)|
| | | |[relativevelocityjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjointblock.md)|
| | | |[revolutejoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint2dblock.md)|
| | | |[revolutejointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejointblock.md)|
| | | |[stickjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/stickjointblock.md)|
| | | |[universaljointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljointblock.md)|
| | | |[uprightjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjointblock.md)|
| | | |[weldjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/weldjointblock.md)|
| | | |[wheeljoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint2dblock.md)|
| | | |[wheeljointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljointblock.md)|


 #  Properties


---  
 #  AngularBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The exponential constant for correcting angular error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The exponential constant for correcting linear error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.md#constraintpositioncorrection)

> What method should be used to fix errors in joints.
> ``` lang=cpp, name=Lightning
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.md)

> The amount of error allowed before position correction takes effect.
> ``` lang=cpp, name=Lightning
> var Slop : Real


---  
 #  Methods


---  
 

 
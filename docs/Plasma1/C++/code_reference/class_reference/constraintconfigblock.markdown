 `Physics`

(NOTE) A block of information for solving a joint (or constraint) type. This is used to configure how one joint is solved independently of another joint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AngularBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#angularbaumgarte-plasma-en)|[safeid32object](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/safeid32object.markdown)|[contactblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/contactblock.markdown)|
| |[ AngularErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#angularerrorcorrection-z)| |[customjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/customjointblock.markdown)|
| |[ LinearBaumgarte](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#linearbaumgarte-plasma-eng)| |[fixedanglejointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/fixedanglejointblock.markdown)|
| |[ LinearErrorCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#linearerrorcorrection-ze)| |[gearjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/gearjointblock.markdown)|
| |[ PositionCorrectionType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#positioncorrectiontype-z)| |[linearaxisjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/linearaxisjointblock.markdown)|
| |[ Slop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/constraintconfigblock.markdown#slop-plasma-engine-documen)| |[manipulatorjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/manipulatorjointblock.markdown)|
| | | |[phygunjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/phygunjointblock.markdown)|
| | | |[positionjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/positionjointblock.markdown)|
| | | |[prismaticjoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjoint2dblock.markdown)|
| | | |[prismaticjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/prismaticjointblock.markdown)|
| | | |[pulleyjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/pulleyjointblock.markdown)|
| | | |[relativevelocityjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/relativevelocityjointblock.markdown)|
| | | |[revolutejoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejoint2dblock.markdown)|
| | | |[revolutejointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/revolutejointblock.markdown)|
| | | |[stickjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/stickjointblock.markdown)|
| | | |[universaljointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/universaljointblock.markdown)|
| | | |[uprightjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/uprightjointblock.markdown)|
| | | |[weldjointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/weldjointblock.markdown)|
| | | |[wheeljoint2dblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljoint2dblock.markdown)|
| | | |[wheeljointblock](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/wheeljointblock.markdown)|


 #  Properties


---  
 #  AngularBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The exponential constant for correcting angular error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The exponential constant for correcting linear error with a penalty impulse.
> ``` lang=cpp, name=Lightning
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Lightning
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#constraintpositioncorrection)

> What method should be used to fix errors in joints.
> ``` lang=cpp, name=Lightning
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> The amount of error allowed before position correction takes effect.
> ``` lang=cpp, name=Lightning
> var Slop : Real


---  
 #  Methods


---  
 

 
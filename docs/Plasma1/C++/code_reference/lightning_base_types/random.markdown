 `Core`

(NOTE) Contains utility functions for random generation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ BellCurve](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#bellcurve-plasma-engine-do)|[ MaxInteger](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#maxinteger-plasma-engine-d)| | |
|[ Boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#boolean-plasma-engine-docu)|[ Seed](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#seed-plasma-engine-documen)| | |
|[ CoinFlip](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#coinflip-plasma-engine-doc)| | | |
|[ DieRoll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#dieroll-plasma-engine-docu)| | | |
|[ DoubleRange](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#doublerange-plasma-engine)| | | |
|[ DoubleReal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#doublereal-plasma-engine-d)| | | |
|[ Integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#integer-plasma-engine-docu)| | | |
|[ Probability](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#probability-plasma-engine)| | | |
|[ Quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#quaternion-plasma-engine-d)| | | |
|[ Constructor](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#random-void)| | | |
|[ Range](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#range-plasma-engine-docume)| | | |
|[ RangeExclusiveMax](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#rangeexclusivemax-plasma-e)| | | |
|[ RangeInclusiveMax](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#rangeinclusivemax-plasma-e)| | | |
|[ Real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#real-plasma-engine-documen)| | | |
|[ Real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#real2-plasma-engine-docume)| | | |
|[ Real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#real3-plasma-engine-docume)| | | |
|[ Rotation](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#rotation-plasma-engine-doc)| | | |
|[ UnitReal2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#unitreal2-plasma-engine-do)| | | |
|[ UnitReal3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#unitreal3-plasma-engine-do)| | | |
|[ Variance](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/random.markdown#variance-plasma-engine-doc)| | | |


 #  Properties


---  
 #  MaxInteger : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

 `read-only` `static`

> Returns the max integer value that can be returned.
> ``` lang=cpp, name=Lightning
> var MaxInteger : Integer


---  
 #  Seed : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> The seed controls what random numbers are generated in a sequence (determanistically) The same seed will always generate the same string of random numbers.
> ``` lang=cpp, name=Lightning
> var Seed : Integer


---  
 #  Methods


---  
 #  BellCurve : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Samples a bell curve with standard normal distribution in the range [0,1] This is equivalent to a Gaussian distribution with standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function BellCurve() : Real
> ``` 


---  
 #  BellCurve : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Samples a bell curve with in the range [center - range, center + range] This uses a standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |range|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function BellCurve(center : Real, range : Real) : Real
> ``` 


---  
 #  BellCurve : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Samples a bell curve in the range [center - range, center + range] with the given standard deviation. Around 68% will lie within the 1st standard deviation.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |range|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |standardDeviation|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function BellCurve(center : Real, range : Real, standardDeviation : Real) : Real
> ``` 


---  
 #  Boolean : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Returns a random boolean value.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Boolean() : Boolean
> ``` 


---  
 #  CoinFlip : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Returns true if the coin flips heads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function CoinFlip() : Boolean
> ``` 


---  
 #  DieRoll : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Randomly rolls a number in the range [1, sides].
> |Name|Type|Description|
> |---|---|---|
> |sides|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function DieRoll(sides : Integer) : Integer
> ``` 


---  
 #  DoubleRange : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)| |
> ||[doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)| |
> ``` lang=cpp, name=Lightning
> function DoubleRange( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  DoubleReal : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)

> Returns a random double real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function DoubleReal() : DoubleReal
> ``` 


---  
 #  Integer : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Returns a random integer in the range of [0, MaxInt].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Integer() : Integer
> ``` 


---  
 #  Probability : [boolean](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/boolean.markdown)

> Takes a given probability that we get a true value.
> |Name|Type|Description|
> |---|---|---|
> |probOfTrue|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Probability(probOfTrue : Real) : Boolean
> ``` 


---  
 #  Quaternion : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.markdown)

> Random unit length quaternion. This is also a unit quaternion.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Quaternion() : Quaternion
> ``` 


---  
 #  Random : Void

 `constructor`

> Default constructor (grabs the random seed)
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Random()
> ``` 


---  
 #  Random : Void

 `constructor`

> Construct a random generator with a specific seed.
> |Name|Type|Description|
> |---|---|---|
> |seed|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Random(seed : Integer)
> ``` 


---  
 #  Range : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> A random Real in the range [min,max].
> |Name|Type|Description|
> |---|---|---|
> |min|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |max|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Range(min : Real, max : Real) : Real
> ``` 


---  
 #  RangeExclusiveMax : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Integer in the range [min, max].
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |max|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function RangeExclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  RangeInclusiveMax : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Integer in the range [min, max)
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |max|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function RangeInclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  Real : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Returns a random real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Real() : Real
> ``` 


---  
 #  Real2 : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

> Randomly generates a Real2 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |maxLength|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real2(minLength : Real, maxLength : Real) : Real2
> ``` 


---  
 #  Real3 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Randomly generates a Real3 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |maxLength|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Real3(minLength : Real, maxLength : Real) : Real3
> ``` 


---  
 #  Rotation : [quaternion](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/quaternion.markdown)

> Random rotation quaternion. This is the same as calling Quaternion()
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function Rotation() : Quaternion
> ``` 


---  
 #  UnitReal2 : [real2](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real2.markdown)

> Generates a unit length Real2.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UnitReal2() : Real2
> ``` 


---  
 #  UnitReal3 : [real3](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real3.markdown)

> Generates a unit length Real3.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function UnitReal3() : Real3
> ``` 


---  
 #  Variance : [doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)

> Integer in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)| |
> ||[doublereal](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/doublereal.markdown)| |
> ``` lang=cpp, name=Lightning
> function Variance( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  Variance : [integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)

> Integer in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> |variance|[integer](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/integer.markdown)| |
> ``` lang=cpp, name=Lightning
> function Variance(base : Integer, variance : Integer) : Integer
> ``` 


---  
 #  Variance : [real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)

> Returns a number in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |variance|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function Variance(base : Real, variance : Real) : Real
> ``` 


---  
 

 
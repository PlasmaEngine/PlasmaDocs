 `Sound`

(NOTE) Generates audio using additive synthesis.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddHarmonic](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.markdown#addharmonic-void)| |[soundnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundnode.markdown)| |
|[ NoteOff](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.markdown#noteoff-void)| | | |
|[ NoteOn](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.markdown#noteon-void)| | | |
|[ RemoveAllHarmonics](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.markdown#removeallharmonics-void)| | | |
|[ StopAllNotes](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/additivesynthnode.markdown#stopallnotes-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  AddHarmonic : Void

> Adds a new harmonic to the additive synth notes. The first value is the multiplier that will be applied to the base frequency, the second is the volume of this harmonic, and the third (the AdsrEnvelope object) contains the envelope-related values.
> |Name|Type|Description|
> |---|---|---|
> |frequencyMultiplier|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |envelope|[adsrenvelope](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/adsrenvelope.markdown)| |
> |type|[SynthWaveType](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/enum_reference.markdown#synthwavetype)| |
> ``` lang=cpp, name=Lightning
> function AddHarmonic(frequencyMultiplier : Real, volume : Real, envelope : AdsrEnvelope, type : SynthWaveType)
> ``` 


---  
 #  NoteOff : Void

> Stops playing all current notes at the specified MIDI value.
> |Name|Type|Description|
> |---|---|---|
> |midiNote|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function NoteOff(midiNote : Real)
> ``` 


---  
 #  NoteOn : Void

> Starts playing a new note. The first parameter is the MIDI note value (range is 0 to 127), and the second is the volume modification that should be applied to this note (a value of 1.0 does not change the volume, while 0.0 would be silence).
> |Name|Type|Description|
> |---|---|---|
> |midiNote|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> |volume|[real](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/lightning_base_types/real.markdown)| |
> ``` lang=cpp, name=Lightning
> function NoteOn(midiNote : Real, volume : Real)
> ``` 


---  
 #  RemoveAllHarmonics : Void

> Removes all current harmonics. You must add at least one harmonic before playing a note.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function RemoveAllHarmonics()
> ``` 


---  
 #  StopAllNotes : Void

> Stops playing all current notes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Lightning
> function StopAllNotes()
> ``` 


---  
 

 
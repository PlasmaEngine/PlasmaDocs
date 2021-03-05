SoundNodes are the objects which create and modify all audio in the Plasma Engine. If you are new to SoundNodes and the SoundNode graph, be sure to read the overview page first.

- [SoundNode Overview ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/soudnode_overview.markdown)
- [SoundNode Graph Tool ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode_graph.markdown)

 # Generating Audio

 ## [GeneratedWaveNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/generatedwavenode.markdown)

Creates audio at a specified pitch using generated audio waves.

 ## [AdditiveSynthNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/additivesynthnode.markdown)

Plays notes at specified pitches using additive synthesis.

 ## [CustomAudioNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/customaudionode.markdown)

Allows the user to pass buffers of audio data directly to the audio engine for output.

 # Volume and Pitch Modifications

 ## [VolumeNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/volumenode.markdown)

Changes the volume of the audio provided by its inputs.

 ## [Panning Node ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/panningnode.markdown)

Changes the volume of the left and right channels of the audio provided by its inputs separately.

 ## [PitchNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/pitchnode.markdown)

Changes the pitch of the audio provided by its inputs.

 ## [EqualizerNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/equalizernode.markdown)

Changes the volume of the audio provided by its inputs in certain frequency ranges.

 ## [CompressorNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/compressornode.markdown)

Applies a compressor filter to the audio provided by its inputs.

 ## [ExpanderNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/expandernode.markdown)

Applies an expander filter to the audio provided by its inputs.

 # Audio Effect Filters

 ## [ReverbNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/reverbnode.markdown)

Applies a simple reverb filter to the audio provided by its inputs.

 ## [LowPassNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/lowpassnode.markdown)

Applies a low pass filter to the audio provided by its inputs (removes high frequencies).

 ## [HighPassNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/highpassnode.markdown)

Applies a high pass filter to the audio provided by its inputs (removes low frequencies).

 ## [BandPassNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/bandpassnode.markdown)

Applies a band pass filter to the audio provided by its inputs (removes frequencies higher and lower than the band).

 ## [DelayNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/delaynode.markdown)

Applies a delay filter to the audio provided by its inputs.

 ## [ChorusNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/chorusnode.markdown)

Applies a chorus filter to the audio provided by its inputs.

 ## [FlangerNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/flangernode.markdown)

Applies a flanger filter to the audio provided by its inputs.

 ## [AddNoiseNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/addnoisenode.markdown)

Adds white noise to the audio provided by its inputs.

 ## [ModulationNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/modulationnode.markdown)

Applies either ring modulation or amplitude modulation to the audio provided by its inputs.

 # Recording Audio

 ## [RecordingNode ](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundnode/recordingnode.markdown)

Saves all audio produced by its inputs to a WAV file. 

 
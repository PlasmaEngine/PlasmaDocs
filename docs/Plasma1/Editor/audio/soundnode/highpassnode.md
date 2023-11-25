# High Pass Node
The [ HighPassNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/highpassnode.md) collects audio data from all of its inputs and applies a high pass filter to it before passing it along to its outputs. 

# Common Uses

- Removing excessive low frequencies
- Combining with white noise and other audio filters to create wind or other sound effects

# Using the HighPassNode

High pass filters leave high frequencies untouched while silencing low frequencies below their cutoff frequency. The only property on the HighPassNode is the `CutoffFrequency`, which sets the frequency at which the filter starts to take effect.

# Related Materials
## Manual
- [soudnode_overview](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/soudnode_overview.md)
- [bandpassnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/bandpassnode.md)
- [lowpassnode](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/lowpassnode.md)

## Code Reference
- [ HighPassNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/highpassnode.md) 

 
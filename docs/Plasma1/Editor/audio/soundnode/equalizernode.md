# Equalizer Node
The [ EqualizerNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/equalizernode.md) collects audio data from all of its inputs and applies several filters to it before passing it along to its outputs, allowing the user to control the loudness of frequencies in specific ranges. 

# Common Uses

- Controlling volume of specific frequencies for either a single sound or several sounds at once

# Using the EqualizerNode

The EqualizerNode controls volume for five separate frequency ranges. The `LowPassGain` value adjusts the volume of frequencies below `80` Hz; `HighPassGain` adjusts volume above `5000` Hz; `Band1Gain` adjusts the volume of frequencies in a band centered at `150` Hz; `Band2Gain` adjusts the band centered at `600` Hz; and `Band3Gain` adjusts the band centered at `2500` Hz.

All five properties can be smoothly changed over time using the `InterpolateAllBands` method.

# Related Materials
## Manual
- [soudnode_overview](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/soudnode_overview.md)

## Code Reference
- [ EqualizerNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/equalizernode.md) 

 
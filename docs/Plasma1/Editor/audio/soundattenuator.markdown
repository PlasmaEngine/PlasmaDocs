# Sound Attenuators
The [ SoundAttenuator ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown) resource controls how a sound played through a [SoundEmitter ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundemitter.markdown) on an object decreases in volume as the object gets further away from a  [SoundListener ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundlistener.markdown). 

# Using SoundAttenuators 


SoundAttenuators can be added to both [SoundCues ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundcue.markdown) and SoundEmitters. If a SoundCue has a SoundAttenuator other than the DefaultNoAttenuation resource attenuator, its settings will be used when the SoundCue is played through any SoundEmitter. Otherwise the settings from the SoundAttenuator on the SoundEmitter will be used. If the SoundEmitter also has DefaultNoAttenuation resource selected, the sound will be heard spatially by SoundListeners (panned to left or right depending on the location of the object), but will not change its volume with distance.

## Attenuation

The volume of sounds are reduced, or attenuated, according to their distance from a relevant SoundListener, using a specified curve. In the real world, as sounds get further away their volume drops off quickly at first, and then slowly. This logarithmic curve is the default setting for SoundAttenuators, but other types of curves can be chosen for custom behaviors.

## Low Pass Filter

Another thing that happens in the real world with distance is that high frequencies are attenuated more quickly than low frequencies. This can be imitated by applying a low-pass filter to the audio. The low-pass filter on SoundAttenuators can be turned off and on depending on the desired sound.


# Related Materials

## Manual
- [SoundEmitter ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundemitter.markdown)
- [SoundListener ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundlistener.markdown)
- [SoundCue ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundcue.markdown)

## Reference
- [ SoundAttenuator ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundattenuator.markdown) 

 
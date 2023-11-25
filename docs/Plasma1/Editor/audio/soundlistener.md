# Sound Listeners
[ SoundListeners ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md), along with [SoundEmitters ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundemitter.md), are responsible for all positional audio in the Plasma Engine.

# Using SoundListeners

The SoundListener component 'hears' all positional audio in a [SoundSpace ](https://github.PlasmaEngine/PlasmaDocsocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundspace.md), using the orientation of the object it's attached to, as if it added a set of ears to that object. For example, if there is a SoundListener component on the Player object, and an object with a SoundEmitter playing a constant sound moves past the player from left to right, the sound will initially play primarily from the user's left speaker and will move to the right speaker as the object moves across the screen. If the SoundEmitter or [SoundCue](https://gitPlasmaEngine/PlasmaDocseroDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundcue.md) is also using a [SoundAttenuator ](https://gitPlasmaEngine/PlasmaDocseroDocs/blob/master/plasma_editor_documentation/plasmamanual/audio/soundattenuator.md) resource, the sound will start quietly and become louder as the object approaches the player, then become quiet again as it moves away. It would sound exactly the same if the player moved past the object instead of the object moving past the player.

The SoundListener component is traditionally placed on the player object (or the camera if the camera uses a first-person POV), as this the allows the player of the game to control the source from which all sounds in the level are heard. It is unusual to have multiple SoundListeners in a single SoundSpace, but if there are the audio that they hear will be combined.

WARNING: New levels have a SoundListener component automatically attached to the GameCamera. If a SoundListener is added to another object the one on the GameCamera must be removed (unless the user is deliberately using two listeners).

If the SoundListener's Active checkBox property is set to `false` in a LightningScript, the SoundListener will not produce any sound. All audio in the SoundSpace will continue to be processed, even if there are no active SoundListeners, so this is not the same as pausing the sounds. 

# Related Materials

## Manual
- [SoundEmitter ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundemitter.md)
- [SoundSpace ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundspace.md)
- [SoundCue ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundcue.md)
- [SoundAttenuator ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundattenuator.md)

## Reference
- [ SoundListener ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/soundlistener.md) 

 
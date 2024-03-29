# Audio Error
*Audio Error: Audio is too loud and is being clipped. Reduce volume or number of sounds to avoid audio problems.*

# Audio Error: Audio is too loud and is being clipped. Reduce volume or number of sounds to avoid audio problems.

## Why does this happen?

## Why does this happen?

All digital audio is represented by oscillating waves that can range in value from -1.0 to 1.0. If some of the waves are very loud, or if too many get added together, mathematically that can result in values outside of this range. Those results must be clamped to 1.0 or -1.0, which means that some of the audio data is lost. This can cause clicks, pops, or static in the audio. 

There are a few different reasons why this might be happening, but the most common reasons are:
- Too many sounds playing
- Volume is too high somewhere (a SoundInstance, a SoundEmitter, a SoundSpace, etc.)
 - Remember that volume adjustments by different objects are multiplied together. If a SoundInstance's Volume is 1.2 and the SoundEmitter's Volume is 1.2 the volume applied to the audio file will be 1.44.

## How can this be fixed?

This is highly dependent on what is happening in the project, but in general there are two solutions; manage the number of active sounds or reduce the volume somewhere. 

If the problem is too many sound effects playing at once, the `InstanceLimit` property on a [SoundTag  ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundtag/) can be used to limit how many effects can play at once. The SoundTag's Compressor settings can be used to reduce the volume of the sound effects when they are too loud.

[SoundNodes ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode.md) such as the [VolumeNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/volumenode/) or [CompressorNode ](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundnode/compressornode.md) can be used to control the overall volume of a [SoundSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundspace.md) or collection of [SoundInstances](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/audio/soundinstance.md).

The best plan, however, is to investigate what is happening with the audio in the project and fix the underlying issues instead of papering over the problem with a quick fix. 

 
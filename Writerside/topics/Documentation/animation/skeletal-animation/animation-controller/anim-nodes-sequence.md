# Play Clip Sequence Node

The *play clip sequence node* is similar to the [play single clip node](anim-nodes-playclip.md), however, instead of playing just a single clip (looped), the sequence node plays at least three clips in a row. One to enter an animation state, one (looped) animation while it stays active, and one to exit the animation state.

Such sequences are common for actions such as jumping or climbing a ladder. The start clip transitions the character from a start state, such as idle or walking into the new state, such as *jumping*. The middle clip is then played as long as the jumping state needs to continue, and once the character hits the ground again, the end clip is played to transition back.

## Properties

See [common properties](anim-nodes-playclip.md#common-properties).

* `StartClip`: The [animation clip](animation-clip-asset.md) to start with. This clip should end on a keyframe from where the `MiddleClips` can continue seemlessly.

* `MiddleClips`: One or multiple animation clips to play after the `StartClip`. Typically these will get looped as long as the node is `Active`. If more than one clip is set, which one to play can be selected using the `MiddleClipIndex` pin. Otherwise a random one will be selected on every iteration.

* `EndClip`: The clip to play after the middle clips are finished. If the node is *looped* this will only happen once the `Active` pin is not triggered anymore.

## Input Pins

See [common input pins](anim-nodes-playclip.md#common-input-pins).

* `MiddleClipIndex`: This pin can be used to select which of the `MiddleClips` to play next. In the video above this is used to select whether the gun should get fired or not.

## Output Pins

See [common output pins](anim-nodes-playclip.md#common-output-pins).

* `OnNextClip`: This pin will get triggered every time a clip finishes and the next middle or end clip starts. This can be used to know for example when the start phase has finished.
  
* `PlayingClipIndex`: This pin outputs the index of the currently playing clip. This value is `0 to N-1` for any of the `N` middle clips. It will be `-1` when the start clip is playing and `-2` when the end clip is playing.

## See Also


* [Animation Controller](Animation-Controller.md)
* [Skeletal Animations](Skeletal-Animation.md)

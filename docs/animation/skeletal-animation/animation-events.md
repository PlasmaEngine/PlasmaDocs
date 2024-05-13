# Animation Events

*Animation events* are markers that are placed in [animation clip assets](animation-clip-asset.md) to indicate that something of interest happens at a certain time during playback.

These events can be used for mundane things like *foot down* markers, in a walking animation, to vital gameplay information like *shot fired* in an attack animation. 

Whenver the Plasma animation system plays back any animation clip, it also inspects all the *event track*. For every event that it encounters, it broadcasts an `plMsgGenericEvent` with `Message` set to the value of the event's name.

If you have a [TypeScript](../../custom-code/typescript/typescript-overview.md) or [Visual Script](../../custom-code/visual-script/visual-script-overview.md) (or [custom C++ components](../../custom-code/cpp/custom-cpp-component.md) that is also an event handler) attached to any parent node of the animated mesh, you can handle this type of event and react with the desired game logic.

![[anim-clip.gif]]
The clip above shows the event track at the bottom of an [animation clip asset](animation-clip-asset.md). 

## See Also


* [Skeletal Animations](skeletal-animation-overview.md)
* [Event Nodes](animation-controller/anim-nodes-events.md)
* [Custom Code](../../custom-code/custom-code-overview.md)
* [Messaging](../../runtime/world/world-messaging.md)

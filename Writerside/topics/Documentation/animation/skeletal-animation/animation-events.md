# Animation Events

*Animation events* are markers that are placed in [animation clip assets](animation-clip-asset.md) to indicate that something of interest happens at a certain time during playback.

These events can be used for mundane things like *foot down* markers, in a walking animation, to vital gameplay information like *shot fired* in an attack animation. 

Whenver the Plasma animation system plays back any animation clip, it also inspects all the *event track*. For every event that it encounters, it broadcasts an `plMsgGenericEvent` with `Message` set to the value of the event's name.

If you have a [TypeScript](TypeScript.md) or [Visual Script](Visual-Script.md) (or [custom C++ components](custom-cpp-component.md) that is also an event handler) attached to any parent node of the animated mesh, you can handle this type of event and react with the desired game logic.

![[anim-clip.gif]]
The clip above shows the event track at the bottom of an [animation clip asset](animation-clip-asset.md). 

## See Also


* [Skeletal Animations](Skeletal-Animation.md)
* [Event Nodes](anim-nodes-events.md)
* [Custom Code](Code.md)
* [Messaging](world-messaging.md)

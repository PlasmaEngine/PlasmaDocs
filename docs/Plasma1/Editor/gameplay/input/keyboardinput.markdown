# Keyboard
The keyboard is a common channel of providing user input to a Plasma project. Keyboard controls are quick and easy to set up, but there are a few details that are important to bear in mind.

# Polling-Based Input vs. Event-Based Input

There are two ways of checking keyboard input in the Plasma Engine: by polling the state of the keyboard (typically in an Update function), known as **polling-based** input, and by connecting to keyboard events, known as **event-based** input. Each has its advantages.

## Polling-Based Input

Polling-based input typically occurs in a callback for an Update event such as [ LogicUpdate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#logicupdate):

<pre><code class="language-csharp" name="Update Connection Example">
function Initialize(init : CogInitializer)
{
  Plasma.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
}
</code></pre>

The keyboard may be polled using a handful of functions on `Plasma.Keyboard`.

### KeyIsDown

The [ KeyIsDown](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboard.markdown#keyisdown-plasma-engine-do) function returns whether the given keyboard key is down on the current frame. It is often used for movement and other actions that are performed over the course of many consecutive frames:

<pre><code class="language-csharp" name="KeyIsDown Example">
if (Plasma.Keyboard.KeyIsDown(Keys.Up))
{
  this.MoveForward();
}
</code></pre>

### KeyIsUp

The [ KeyIsUp](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboard.markdown#keyisup-plasma-engine-docu) function returns whether the given keyboard key is *not* down on the current frame. It is sometimes used in combination with **KeyIsDown** in movement code:

<pre><code class="language-csharp" name="KeyIsUp Example">
if (Plasma.Keyboard.KeyIsDown(Keys.Right) && Plasma.Keyboard.KeyIsUp(Keys.Left))
{
  this.TurnCounterClockwise();
}

if (Plasma.Keyboard.KeyIsDown(Keys.Left) && Plasma.Keyboard.KeyIsUp(Keys.Right))
{
  this.TurnClockwise();
}
</code></pre>

### KeyIsPressed

The [ KeyIsPressed](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboard.markdown#keyispressed-plasma-engine) function returns whether the given keyboard key is down on the current frame *and* was up on the previous frame. It is often used for discrete actions, like activating character abilities and interacting with menus:

<pre><code class="language-csharp" name="KeyIsPressed Example">
if (Plasma.Keyboard.KeyIsPressed(Keys.Space))
{
  this.Jump();
}
</code></pre>

### KeyIsReleased

The [ KeyIsReleased](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboard.markdown#keyisreleased-plasma-engin) function returns whether the given keyboard key is up on the current frame, but was down on the previous frame. It is often used to end actions or processes that were started by the same key in a KeyIsPressed check:

<pre><code class="language-csharp" name="KeyIsReleased Example">
if (Plasma.Keyboard.KeyIsReleased(Keys.Space))
{
  this.EndJump();
}
</code></pre>

Such queries are usually performed in a function that is called every frame, once per frame, such as an Update function; polling for input in this way is also called **frame-based input**. However, the keyboard can be polled at any time. For instance, one might check whether a certain key is held in a [ CollisionStarted](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#collisionstarted) callback, to determine whether some special action should occur:

<pre><code class="language-csharp" name="Collision Polling Example">
function OnCollisionStarted(event : CollisionEvent)
{
  if (Plasma.Keyboard.KeyIsDown(Keys.Z))
    this.AttemptDealDamage(event.OtherObject);
}
</code></pre>

NOTE: Beware that the LogicUpdate event is not dispatched on a paused TimeSpace. If input polling is performed in a LogicUpdate callback, it won't happen while the game is paused. This may result in a scenario where LogicUpdate is used to pause the game, and then it becomes impossible to unpause. For this reason, it is usually best to pause the game using event-based input, or by polling the keyboard via another event, such as [ FrameUpdate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#frameupdate), or in the LogicUpdate of another Space.

## Event-Based Input

The keyboard dispatches a set of handy events that can be used for keyboard input:

<pre><code class="language-csharp" name="Keyboard Connection Example">
function Initialize(init : CogInitializer)
{
  Plasma.Connect(Plasma.Keyboard, Events.KeyDown, this.OnKeyDown);
  Plasma.Connect(Plasma.Keyboard, Events.KeyUp, this.OnKeyUp);
  Plasma.Connect(Plasma.Keyboard, Events.KeyRepeated, this.OnKeyRepeated);
}
</code></pre>

The [ KeyboardEvent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboardevent.markdown) object that gets sent with these events specifies which key triggered the event, along with other relevant information, such as whether any of various modifier keys was held when the event was dispatched, etc.

### KeyDown

When any key on the keyboard is pressed, the [ KeyDown](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#keydown) event is dispatched that frame:

<pre><code class="language-csharp" name="KeyDown Example">
function OnKeyDown(event : KeyboardEvent)
{
  if (event.Key == Keys.R && event.CtrlPressed)
    this.RestartLevel();
}
</code></pre>

### KeyUp

When any key on the keyboard is released, the [ KeyUp](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#keyup) event is dispatched that frame:

<pre><code class="language-csharp" name="KeyUpExample">
function OnKeyUp(event : KeyboardEvent)
{
  if (event.Key == Keys.Shift)
    this.EndChargingWeapon();
}
</code></pre>

### KeyRepeated

When any key on the keyboard is held long enough for the operating system to send its "repeated" event, the [ KeyRepeated](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#keyrepeated) event begins being dispatched. The delays before this begins and between dispatches are determined by the operating system:

<pre><code class="language-csharp" name="KeyRepeated Example">
function OnKeyRepeated(event : KeyboardEvent)
{
  if (event.Key == Keys.Back)
    this.Backspace();
}
</code></pre>

# Timing

Every frame, all keyboard events are dispatched at the beginning of the frame before any update events are dispatched. If it is desired that any code that is called from an Update function be run before the effects of some keypress are considered, then either polling-based input should be used instead of event-based input, or the keypress should be cached, and the cached data should be used later.

# What to Use

First and foremost, in many cases, there will be no noticeable performance difference between using polling-based input and using event-based input. For example, when creating a simple prototype or adding a quick debugging feature, it is often best to use whichever method is easiest for the developer implementing it.

However, when performance does become an issue, or when scalability is a concern, knowing which input method to use is important. To decide whether to use polling-based or event-based input, begin by answering these guideline questions:

**Is this component already connected to an update event?**
- **Yes**: polling may be better
- **No**: consider events

Some of the performance impact in frame-based input comes from the act of polling, but some of it comes from the mere fact of being connected to an update event. If a component's update event connection overhead is already considered acceptable, then the added overhead of input polling may not be a problem.

**How many instances of this component are likely to be alive at once?**
- **A lot**: events may be better
- **Not many**: consider polling

Performance can suffer noticeably if a large number of objects are simultaneously connected to update events, especially if they're running complex logic. If there will be more than about a few hundred instances of a component all running at once, it may be wise to consider using event-based input instead of frame-based input. Of course, this number will vary greatly with factors such as the complexity of the logic being run and the capabilities of the user's computer.

**How much time is likely to elapse between relevant inputs?**
- **A long time**: events may be better
- **Not long**: consider polling

Update events are generally dispatched every frame. Keyboard events, on the other hand, are only dispatched when the keyboard is used. For this reason, event-based input has the potential to be more efficient than frame-based input, especially when checking for an input that is expected to occur only rarely or sporadically.

**How hard will it be to do this logic using events?**
- **Very hard**: polling may be better
- **Not very hard**: consider events

Some input tasks don't lend themselves to being done with event-based input. For example, it can be awkward to make keyboard events, which are dispatched only on keyboard state changes, work with character movement code, which generally should apply its changes every frame.

#  Related Materials
##  Manual
- [ Events & Connections](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/scripting/eventsandconnections.markdown)
- [ Components](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/architecture/components.markdown)

##  Code Reference
- [ Keyboard](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboard.markdown)
- [ KeyboardEvent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/keyboardevent.markdown) 

 
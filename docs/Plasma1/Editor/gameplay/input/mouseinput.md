# Mouse
Along with the keyboard and gamepads, the mouse is a common channel of providing user input to a Plasma project. Mouse controls are easy to set up, but there are a few different input styles to consider.

# Using the Mouse

The mouse can either be used as a cursor controller, for tracking a specific position and pointing at and clicking on objects and buttons, etc., or it can be used as a direct input device, just like a keyboard or a gamepad.

## Cursor Control

**Cursor control**, also known as *point-and-click* control, is usually what is used for mouse-driven GUIs. It is mostly focused on the use of the mouse to manipulate the position of a cursor in a 2D plane. Cursor control typically makes heavy use of the [ Reactive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/reactive.md) component to receive mouse events sent directly to interactive objects, such as buttons.


## Direct Mouse Control

**Direct mouse control** is commonly used for first-person camera controls, and anything else that is concerned with the frame-to-frame movement deltas of the mouse, and the state changes of its buttons and scroll wheel, rather than with the position of a cursor. When using direct mouse control, mouse event connections should be made on the Space or the camera viewport (rather than on individual interactive objects, as with cursor control).



# Event-Based Input vs. Polling-Based Input

Whether the mouse is used for cursor control or direct control, in any case, there are two ways of using mouse input in the Plasma Engine: by connecting to mouse events, known as **event-based** input, by polling the state of the mouse (typically in an Update function), known as **polling-based** input. Each has its advantages.

## Events

Mouse events are dispatched as the mouse is used, and the position of the mouse cursor determines the targets of these events. When the cursor is positioned over an cog with the [ Reactive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/reactive.md) component, that cog receives mouse events.

In addition, mouse events are also sent to viewports. When a mouse event occurs in a viewport, it is dispatched to the cog with the [ Camera](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/camera.md) component and the cog with the [ CameraViewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.md) component that represent that viewport. (Events are not dispatched doubly if both components are on the same cog, as is commonly the case.)

NOTE: A **mouse event target** is anything that can receive a mouse event. Mouse event targets are spaces, cogs with the Camera component, cogs with the CameraViewport component, and cogs with the Reactive component.

Here is an example of the use of mouse events, showing two different event connections, one to the space and one to the Reactive object itself:

<pre><code class="language-csharp" name="Mouse Event Demonstration">
class MouseEventDemonstration : LightningComponent
{
  [Dependency] var Transform : Transform;
  [Dependency] var Reactive : Reactive;
  
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.Space, Events.LeftMouseDown, this.OnLeftMouseDown);
    Plasma.Connect(this.Owner, Events.RightMouseDown, this.OnRightMouseDown);
  }
  
  function OnLeftMouseDown(event : ViewportMouseEvent)
  {
    // when the left mouse button is pressed anywhere,
    // make a cube at the mouse's world position
    var mousePosition = event.ToWorldZPlane(0);
    var cube = this.Space.CreateAtPosition(Archetype.Cube, mousePosition);
    // delay five seconds and then destroy the cube
    var destroySeq = Action.Sequence(cube.Actions);
    Action.Delay(destroySeq, 5);
    Action.Call(destroySeq, cube.Destroy);
  }
  
  function OnRightMouseDown(event : ViewportMouseEvent)
  {
    // when the right mouse button is pressed on this object,
    // make it a little bigger
    this.Transform.Scale = this.Transform.Scale * 1.1;
  }
}
</code></pre>

This component's dependency on **Reactive** requires that the object it is attached to has that component as well. Thus, whenever the left mouse button is pressed with the cursor over an object with this component, the `OnLeftMouseDown` function will be called. Additionally, whenever the right mouse button is pressed *anywhere* in the viewport showing this component's space, the `OnRightMouseButton` function will be called.


### List of Mouse Events

There are a number of mouse events that are dispatched to mouse event targets:

<pre><code class="language-csharp" name="Mouse Event Connections">
function Initialize(init : CogInitializer)
{
  Plasma.Connect(this.Owner, Events.MouseUpdate,       this.OnMouseUpdate);

  Plasma.Connect(this.Owner, Events.MouseEnter,        this.OnMouseEnter);
  Plasma.Connect(this.Owner, Events.MouseExit,         this.OnMouseExit);
  Plasma.Connect(this.Owner, Events.MouseEnterPreview, this.OnMouseEnterPreview);

  Plasma.Connect(this.Owner, Events.MouseMove,         this.OnMouseMove);
  Plasma.Connect(this.Owner, Events.MouseScroll,       this.OnMouseScroll);
  
  Plasma.Connect(this.Owner, Events.MouseDown,         this.OnMouseDown);
  Plasma.Connect(this.Owner, Events.MouseUp,           this.OnMouseUp);
  
  Plasma.Connect(this.Owner, Events.LeftMouseDown,     this.OnLeftMouseDown);
  Plasma.Connect(this.Owner, Events.LeftMouseUp,       this.OnLeftMouseUp);
  
  Plasma.Connect(this.Owner, Events.RightMouseDown,    this.OnRightMouseDown);
  Plasma.Connect(this.Owner, Events.RightMouseUp,      this.OnRightMouseUp);
  
  Plasma.Connect(this.Owner, Events.MiddleMouseDown,   this.OnMiddleMouseDown);
  Plasma.Connect(this.Owner, Events.MiddleMouseUp,     this.OnMiddleMouseUp);

  Plasma.Connect(this.Owner, Events.LeftClick,         this.OnLeftClick);
  Plasma.Connect(this.Owner, Events.RightClick,        this.OnRightClick);
  Plasma.Connect(this.Owner, Events.MiddleClick,       this.OnMiddleClick);

  Plasma.Connect(this.Owner, Events.DoubleClick,       this.OnDoubleClick);
}
</code></pre>

Each of these events is a [ ViewportMouseEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md). This event contains various relevant mouse data, such as the position of the cursor and the states of its buttons.

#### MouseUpdate

Every frame that the mouse is over a mouse event target, the [ MouseUpdate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mouseupdate) event is dispatched to that target:

<pre><code class="language-csharp" name="MouseUpdate Example">
function OnMouseUpdate(event : ViewportMouseEvent)
{
  // move this object to the mouse position
  this.Transform.Translation = event.ToWorldZPlane(0);
}
</code></pre>

#### MouseEnter, MouseExit, and MouseEnterPreview

When the mouse cursor "enters" a mouse event target (that is, when it goes from not being over the target to being over it from the perspective of the viewport showing it) the [ MouseEnter](https://github.PlasmaEngine/PlasmaDocsocs/blob/master/code_reference/event_reference.md#mouseenter) event is dispatched to that target that frame. Likewise, when the cursor "exits" a target (it goes from over it to not over it) the [ MouseExit](https://github.PlasmaEngine/PlasmaDocseroDocs/blob/master/code_reference/event_reference.md#mouseexit) event is dispatched to that target that frame.

As the mouse cursor enters a mouse event target, if it is simultaneously exiting another one, the [ MouseEnterPreview](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mouseenterpreview) event is dispatched that frame to the target being entered. This event is dispatched *immediately before* the **MouseExit** and subsequent **MouseEnter** events are dispatched, in the same frame.

For example, this code snippet connects to two different cogs, `CogA` and `CogB` (declared elsewhere in the script), for these events:

<pre><code class="language-csharp" name="MouseEnter, MouseExit, and MouseEnterPreview Examples">
function Initialize(init : CogInitializer)
{
  Plasma.Connect(this.CogA, Events.MouseExit, this.OnMouseExit);
  Plasma.Connect(this.CogB, Events.MouseEnter, this.OnMouseEnter);
  Plasma.Connect(this.CogB, Events.MouseEnterPreview, this.OnMouseEnterPreview);
}

function OnMouseExit(event : ViewportMouseEvent)
{
  Console.WriteLine("Exiting `this.CogA.Name`");
}

function OnMouseEnter(event : ViewportMouseEvent)
{
  Console.WriteLine("Entering `this.CogB.Name`");
}

function OnMouseEnterPreview(event : ViewportMouseEvent)
{
  Console.WriteLine("About to enter `this.CogB.Name`");
}
</code></pre>

Here is the console output when the mouse moves from `CogA` to `CogB`:

<pre><code name="MouseEnter, MouseExit, and MouseEnterPreview Console Output>
About to enter CogB
Exiting CogA
Entering CogB
</code></pre>

MouseEnterPreview is useful when there is code that should be run before the MouseExit and MouseEnter callbacks are executed.

#### MouseMove and MouseScroll

Every frame that the mouse **moves** while the cursor is over a mouse event target, the [ MouseMove](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mousemove) event is dispatched to that target. When the mouse is **scrolled** while the cursor is over a mouse event target, the [ MouseScroll](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mousescroll) event is dispatched to that target:

<pre><code class="language-csharp" name="MouseMove and MouseScroll Examples">
function OnMouseMove(event : ViewportMouseEvent)
{
  // move the camera an amount equal to the
  // mouse's movement vector
  this.PanCamera(event.Movement);
}

function OnMouseScroll(event : ViewportMouseEvent)
{
  // zoom the camera an amount equal to the
  // Y component of the scroll vector
  this.Zoom(event.Scroll.Y);
}
</code></pre>

#### Down and Up Events

When any mouse button is **pressed** while the cursor is over a mouse event target, the [ MouseDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mousedown) event is dispatched to that target. Likewise, when any mouse button is **released** while the cursor is over a mouse event target, the [ MouseUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#mouseup) event is dispatched to that target.

**MouseDown** and **MouseUp** are useful when writing controls that can be bound to any mouse button. To determine which mouse button was pressed or released, just check the `Button` field on the ViewportMouseEvent object that is sent with the event:

<pre><code class="language-csharp" name="MouseDown and MouseUp Examples">
function OnMouseDown(event : ViewportMouseEvent)
{
  if (event.Button == this.LaserButton)
    this.BeginChargingLaser();
  else if (event.Button == this.ShieldButton)
    this.RaiseShields();
  else if (event.Button == this.CameraPanningButton)
    Plasma.Connect(this.Space, Events.MouseMove, this.OnMouseMove);
}

function OnMouseUp(event : ViewportMouseEvent)
{
  if (event.Button == this.LaserButton)
    this.FireLaser();
  else if (event.Button == this.ShieldButton)
    this.LowerShields();
  else if (event.Button == this.CameraPanningButton)
    Plasma.Disconnect(this.Space, Events.MouseMove, this);
}
</code></pre>

Plasma also has specific events for [ LeftMouseDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#leftmousedown) and [ LeftMouseUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#leftmouseup), [ RightMouseDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#rightmousedown) and [ RightMouseUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#rightmouseup), and [ MiddleMouseDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#middlemousedown) and [ MiddleMouseUp](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#middlemouseup), which are dispatched only when the corresponding button is pressed or released:

<pre><code class="language-csharp" name="Other Down and Up Examples">
function OnLeftMouseDown(event : ViewportMouseEvent)
{
  this.BeginChargingLaser();
}

function OnRightMouseUp(event : ViewportMouseEvent)
{
  this.LowerShields();
}

function OnMiddleMouseDown(event : ViewportMouseEvent)
{
  Plasma.Connect(this.Space, Events.MouseMove, this);
}
</code></pre>

#### Click Events

When a mouse button is both **pressed** and **released** over the same object, that object is said to have been //clicked//. Click events are commonly used for UI elements, such as buttons. Plasma dispatches [ LeftClick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#leftclick), [ RightClick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#rightclick), and [ MiddleClick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#middleclick) events:

<pre><code class="language-csharp" name="Click Examples">
function OnLeftClick(event : ViewportMouseEvent)
{
  // perform whatever effect this button does
  this.ExecuteButtonFunction();
}

function OnRightClick(event : ViewportMouseEvent)
{
  // open the context menu for this object
  this.OpenContextMenu();
}

function OnMiddleClick(event : ViewportMouseEvent)
{
  // close this window
  this.CloseWindow();
}
</code></pre>

#### DoubleClick

When a mouse event target is double-clicked, the [ DoubleClick](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#doubleclick) event is dispatched to that target:

<pre><code class="language-csharp" name="DoubleClick Example">
function OnDoubleClick(event : ViewportMouseEvent)
{
  if (event.Button == this.LaserButton)
    this.ReloadLaser();
  else if (event.Button == this.ShieldButton)
    this.RebootShields();
}
</code></pre>

NOTE: The timing of the two clicks involved in a double click is defined by the user's operating system.

## Polling-Based Input

Polling-based input typically occurs in a callback for an [ Update event](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/updateevent.md) such as [ LogicUpdate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/event_reference.md#logicupdate):

<pre><code class="language-csharp" name="Update Connection Example">
function Initialize(init : CogInitializer)
{
  Plasma.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
}

function OnLogicUpdate(event : UpdateEvent)
{
  // check for mouse input here
}
</code></pre>

The mouse may be polled via the global [ Mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md) object, which can be found at `Plasma.Mouse`; of interest to mouse input are its `CursorMovement`, `RawMovement`, and `ClientPosition` properties and its `IsButtonDown` function.

### CursorMovement, RawMovement, and ClientPosition

[ RawMovement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#rawmovement-plasma-engine) represents the amount of movement detected this frame by the mousing device. [ ClientPosition](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#clientposition-plasma-engi) gives the screen-space cursor position in pixels, as computed by the OS. ClientPosition is relative to the upper left pixel of the Plasma client (application), which is (0, 0), with X and Y increasing to the right and down respectively. The [ CursorMovement](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#cursormovement-plasma-engi) property is computed by Plasma as the difference in the ClientPosition between the current frame and the previous frame.

NOTE: CursorMovement and RawMovement often differ because the final position of the cursor depends on OS settings.

The ClientPosition property is given in screen space, but it may be helpful to convert it to another coordinate basis, such as world space. The [ CameraViewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.md) component has handy functions for performing such changes of basis:

<pre><code class="language-csharp" name="ClientPosition to World Space Example">
function OnLogicUpdate(event : UpdateEvent)
{
  // mouse position in screen space
  var clientPosition = Plasma.Mouse.ClientPosition;
  // mouse position in world space (at Z = 0)
  var mouseWorldPosition = this.CameraViewport.ScreenToWorldZPlane(clientPosition, 0);

  // move this object to the mouse's world position
  this.Transform.Translation = mouseWorldPosition;
}
</code></pre>

 ###  IsButtonDown

The [ IsButtonDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md#isbuttondown-plasma-engine) function returns whether the given mouse button is down on the current frame. It closely parallels the [ KeyIsDown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md#keyisdown-plasma-engine-do) function on the [ Keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md) object:

<pre><code class="language-csharp" name="IsButtonDown Example">
function OnLogicUpdate(event : UpdateEvent)
{
  // if the mouse look button is held, turn the camera with the mouse's movement
  if (Plasma.Mouse.IsButtonDown(this.MouseLookButton))
  {
    this.RotateCamera(Plasma.Mouse.CursorMovement);
  }
}
</code></pre>

# What to Use

Whether direct control or cursor control is used, event-based input and polling-based input may have performance differences. As is the case with [ Keyboard Input](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/gameplay/input/keyboardinput.md#what-to-use), the difference will often be very small, so sometimes it is best to use whichever method is easiest for the developer, but knowing how to decide which input method to use is always important.

To decide whether a component should use event-based mouse input or polling-based mouse input, begin by answering these guideline questions:

**Is the mouse being used for cursor control or direct mouse control?**

- **[Cursor control](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/gameplay/input/mouseinput/.md#cursor-control)**: mouse events are probably better
- **[direct mouse control](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/gameplay/input/mouseinput/.md#direct-mouse-control)**: either may work

The nature of a cursor-driven interface is well-suited to being controlled by mouse events, and is often awkward and impractical to implement with polling.

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

Because mouse events are only dispatched when the mouse is used (other than [ MouseUpdate](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++.md#mouseupdate)), event-based input has the potential to be more efficient than frame-based input, especially when checking for an input that is expected to occur only rarely or sporadically.

# Related Materials
## Manual
- [ Keyboard Input](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/gameplay/input/keyboardinput.md#what-to-use)

## Code Reference
- [ Mouse](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/mouse.md)
- [ ViewportMouseEvent](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/viewportmouseevent.md)
- [ Reactive](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/reactive.md)
- [ CameraViewport](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/cameraviewport.md)
- [ Camera](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/camera.md)
- [ Keyboard](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/keyboard.md)


 
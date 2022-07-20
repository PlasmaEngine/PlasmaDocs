# Menus

This lesson covers the creation of menus in the Plasma Engine.

# Learning Objectives

- Using Plasma's UI system to create graphical menus
- Learning how to use a button interface to switch between levels

# Project Setup
- Create a new project using the Empty 2D Project template

Making a menu, HUD, or simple title screen in Plasma is easy when you start with the built-in UI level template. Let's make a simple game with a title screen, a main menu, and a basic gameplay level.

(NOTE) **What's a Widget?** In this tutorial, you'll encounter the word **widget**. In short, a widget object is a UI element. Plasma widgets object include //points of interaction//, like buttons and sliders, as well as static elements, like text labels and layouts containing other widgets object. What all widgets object have in common is the [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown) component, which each one has. All graphical user interfaces (or **GUIs**) created with Plasma's UI system, whether they're title screens, main menus, or anything else, are composed of widgets object.

![Level Flow](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/LevelUIFlow.png)

We'll start with the title screen.

# Creating a Title Screen
- Command : Add Resource
- Create a Level resource using the Ui Level template and name it `TitleScreen`

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/UILevel.PNG)


The UI level template includes a RootWidget object object, complete with all the special components that make it tick, such as [ UiRootWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uirootwidget.markdown) and `UiRenderer`. It also comes with a few placeholder sprites that we won't be using.



![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/UILevelObjects.PNG)


- In the `Objects Window`
- Under RootWidget object
- Select : the three Sprite object objects
- Command : Delete

Our title screen will consist of white text against a dark background. The background color can be changed through the RootWidget:

- Select : RootWidget object
- In the `Properties Window`
- Under [ UiRootWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uirootwidget.markdown)
- Set LocalColor  to `[R:36, G:36, B:36, A:1.00]`
- Remove Component : [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Add Component : [UiFillLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uifilllayout.markdown)

It's time to make our first widget object: a text label. The best way to make widgets object is to instantiate them from archetypes, and Plasma comes with some archetypes that are just for use in UI creation. These can be found in the `Library Window`, but you'll have to **change libraries** to find them.

- In the `Library Window`
- Open the Library enum list menu
- Select the `UiWidget` library
- Under Archetype 
- `Left drag` `UiSpriteText` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSpriteText` instance on top of RootWidget object


![Adding a UiSpriteText to the RootWidget](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/MenuCreateText.gif)

- In the `Properties Window`
- Rename the UiSpriteText object to `Title`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Under the **Layout** group
- Set HorizontalAlignment enum to `Center`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set TextAlign enum to `Center`

NOTE: The `UiWidget` component's `VerticalAlignment` and `HorizontalAlignment` properties determine where the text widget object's area is positioned within its parent layout (in this case, the RootWidget object). The `SpriteText` component's `TextAlign` property, on the other hand, determines where the text itself is positioned within its own area.

- In the `Properties Window`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `50`
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set MarginTop  to `180`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Font enum to `NotoSans-Bold`
- Set FontSize  to `36`
- Set Text  to something pretentious

(NOTE) **Why Just Y?** Normally in our tutorials, when we want you to set just one part of a vector-type property, we direct you to set the whole thing at once (for example, //Set Translation  to `[0, -5, 0]`//). But above, you are explicitly directed to set just the Y part of the Size  property. The reason is that, a few lines later, when we set the SizePolicyX enum property to `Flex`, it causes the parent layout to "take over" the X part of the Size  property, meaning that any changes that we made to it would overwritten immediately. You'll see this sort of thing throughout Plasma's UI system and our tutorials covering it.


![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/MenuTitle.png) 

*Title screen so far, with hierarchy for reference*

- Select : Title object
- Command : [ Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- Select : the new copy of Title object
- In the `Properties Window`
- Rename the copy of Title object to `Subtitle`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set LocalColor  to `[R:255, G:255, B:255, A:0.50]`
- Under the **Layout** group
- Set MarginTop  to `0`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Font enum to `NotoSans-Regular`
- Set FontSize  to `24`
- Set Text  to something longer and perhaps more pretentious
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `33`

** ADD IMAGE **


*Title screen, continued, with hierarchy for reference*


- Select : Subtitle object
- Command : [ Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- In the `Properties Window`
- Rename the copy of Subtitle object to `StartText`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set LocalColor  to `[R:255, G:255, B:255, A:1.00]`
- Under the **Layout** group
- Set VerticalAlignment enum to `Bottom`
- Set MarginTop  to `0`
- Set MarginBottom  to `180`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Font enum to `NotoSans-Bold`
- Set FontSize  to `16`
- Set Text  to `Click to Start`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `22`

The StartText object says //Click to Start//, but of course clicking won't do anything yet. We'll add that functionality soon, but for now, there's just one more finishing touch to apply to the appearance of the title screen.

- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSprite` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSprite` instance on top of RootWidget object
- In the `Properties Window`
- Rename the UiSprite object to `HorizontalLine`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `2`
- Set LocalColor  to `[R:255, G:0, B:0, A:1.00]`
- Disable 'InLayout'
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set MarginLeft  to `20`
- Set MarginTop  to `218`
- Set MarginRight  to `20`

(NOTE) **Hierarchy Render Order:** If your game's title contains a letter that has a descender (such as a lowercase //y//), the red horizontal line will be rendered on top of it. To correct this, just move the HorizontalLine object object to the top of its hierarchy in the `Objects Window`:  This works because, while hierarchy order doesn't affect the way that widgets object are laid out in a `UiFillLayout`, it does still determine the order in which [ Sprites](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sprite.markdown) and [ SpriteTexts](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown) are rendered by a `UiRenderer`.


** ADD IMAGE **

*The complete layout of the title screen, with hierarchy for reference*


Now for the main menu.

# Creating a Main Menu

The main menu should contain four buttons:

* **Start Game**, which loads the gameplay level

* **Credits**, which loads the credits level
  - The credits level should contain a **Return to Main Menu** button, which loads the main menu level

*  **Return to Title**, which loads the title screen level

* **Quit Game**, which exits the game

Let's get started.

- Command : Add Resource
- Create a Level resource using the {nav icon=clone, name="Ui Level"} template and name it `MainMenu`
- In the `Objects Window`
- Under RootWidget object
- [ Delete](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#delete) : the three Sprite object objects
- Select : RootWidget object
- In the `Properties Window`
- Under [ UiRootWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uirootwidget.markdown)
- Set LocalColor  to `[R:64, G:25, B:25, A:1.00]`
- Remove Component : [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Add Component : [ UiFillLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uifilllayout.markdown)
- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSprite` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSprite` instance on top of RootWidget object
- In the `Properties Window`
- Rename the UiSprite object to `MenuWindow`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set Size  to `[200, 250]`
- Set LocalColor  to `[R:255, G:255, B:255, A:0.10]`
- Under the **Layout** group
- Set VerticalAlignment enum to `Center`
- Set HorizontalAlignment enum to `Center`
- Add Component : [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Under [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Set PaddingLeft  to `4`
- Set PaddingTop  to `4`
- Set PaddingRight  to `4`
- Set PaddingBottom  to `4`
- Set Spacing  to `[0, 4]`

** ADD IMAGE **

*Empty menu window for the main menu, with hierarchy for reference*


- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSpriteText` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSpriteText` instance on top of MenuWindow object
- In the `Properties Window`
- Rename the UiSpriteText object to `MenuTitle`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `41`
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Main Menu`
- Set FontSize  to `30`
- Set TextAlign enum to `Center`

** ADD IMAGE **

*Main menu, continued, with hierarchy for reference*

The menu's window is good to go.

## Adding Buttons

Now to make our first button, the *Start Game* button. When we're done with it, we'll duplicate it three times and modify the duplicates to match the buttons we want the menu to have.

- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSprite` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSprite` instance on top of MenuWindow object
- In the `Properties Window`
- Rename the UiSprite object to `StartGameButton`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set LocalColor  to `[R:255, G:255, B:255, A:0.10]`
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set SizePolicyY enum to `Flex`
- Add Component : [ UiFillLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uifilllayout.markdown)
- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSpriteText` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSpriteText` instance on top of StartGameButton object
- Rename the UiSpriteText object to `ButtonText`
- Under [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `33`
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set VerticalAlignment enum to `Center`
- Under [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Start Game`
- Set Font enum to `NotoSans-Bold`
- Set FontSize  to `24`
- Set TextAlign enum to `Center`

** ADD IMAGE **

*The main menu with the first button (work in progress), with hierarchy for reference*

(NOTE) **Why's Everything Orange?** You may notice that some of the objects in the Objects Window are shown in orange text. Plasma uses this coloring scheme to denote an object that is //an instance of an archetype, but whose property values differ from the archetype it was created from//. Every object we've created so far has been instantiated from archetypes, which we then proceeded to modify. If you want an object's name to be printed in the same manner as the rest of the objects, just select it and clear its Archetype  field in the `Properties Window`. Then it won't be considered an archetype instance anymore.

The button's outward appearance is mostly complete, but we need to give it a Lightning component that gives it its functionality.

- Command : [ Add Resource](https://plasmaengine.github.io/PlasmaDocs/Manual/editor/editorcommands/resourceadding.markdown)
- Create a LightningScript resource using the Component template template and name it `LoadLevelOnClick`
- Update the `LoadLevelOnClick` script to the following:

<pre><code class="language-csharp" name="LoadLevelOnClick">
class LoadLevelOnClick : LightningComponent
{
  [Property]
  var LevelToLoad : Level;
  
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.Owner, Events.LeftClick, this.OnLeftClick);
  }
  
  function OnLeftClick(event : ViewportMouseEvent)
  {
    this.Space.LoadLevel(this.LevelToLoad);
  }
}
</code></pre>

Plasma's UI system sends the [ LeftClick](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#leftclick) event to every **interactive** widget object (that is, every game object whose [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown) component's `Interactive` property is set to `true`) when it is left-clicked. This component uses that event to load a level of our choice, making it perfect for our menu buttons (and more). But in addition to the functionality offered by this component, we can also add some helpful feedback to the button with a couple more core Lightning components: `UiHighlight`, which changes a button's color when it is hovered over or clicked on, and `UiChangeCursor`, which makes a button change the [ mouse cursor](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/enum_reference.markdown#cursor) when it is hovered over.

- Select : StartGameButton object
- In the `Properties Window`
- Add Component : `UiHighlight`
- Add Component : `UiChangeCursor`
- Add Component : `LoadLevelOnClick`
- Under `UiHighlight`
- Set MouseHoverColor  to `[R:255, G:255, B:255, A:0.20]`
- Set MouseDownColor  to `[R:0, G:0, B:0, A:0.10]`
- Set AnimateTime  to `0.06`
- Under `UiChangeCursor`
- Set Cursor enum to `Hand`

** ADD IMAGE **

Now we'll just duplicate this button a few times.

- [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate) : StartGameButton object three times

** ADD IMAGE **

*The menu with four copies of the Start Game button, with hierarchy for reference*

- Set the Text  properties of the [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown) components of the ButtonText object objects to match the following: ** ADD IMAGE **
- Rename the StartGameButton object objects to match the following: ** ADD IMAGE **

The menu is nearly complete; pretty much all that's left to do is to create the levels that the buttons will link to, and then hook them up.

# Creating a Gameplay Level

We'll just throw something together real quick to make a gameplay level. It won't be anything to write home about, but it will be adequate for our needs.

- Command : Add Resource
- Create a Level resource using the {nav icon=clone, name="2D Level"} template and name it `GameplayLevel`
- Command : Add Resource
- Create a LightningScript resource using the Component template template and name it `KeyboardMovement`
- Update the `KeyboardMovement` script to the following:

<pre><code class="language-csharp" name="KeyboardMovement">
class KeyboardMovement : LightningComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var Speed : Real = 8;
  
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }
  
  function OnLogicUpdate(event : UpdateEvent)
  {
    var movement = Real3.Zero;
    
    if (Plasma.Keyboard.KeyIsDown(Keys.Right))
      movement += Real3.XAxis;
    if (Plasma.Keyboard.KeyIsDown(Keys.Left))
      movement -= Real3.XAxis;
    if (Plasma.Keyboard.KeyIsDown(Keys.Up))
      movement += Real3.YAxis;
    if (Plasma.Keyboard.KeyIsDown(Keys.Down))
      movement -= Real3.YAxis;
    
    this.Transform.WorldTranslation += movement * this.Speed * event.Dt;
  }
}
</code></pre>

- Select : Renderer object
- In the `Properties Window`
- Under `ForwardRenderer`
- Set ClearColor  to `[R:51, G:89, B:128, A:1.00]`
- Command : [CreateSprite](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#createsprite)
- In the `Properties Window`
- Rename the Sprite object to `Player`
- Add Component : `KeyboardMovement`
- Under [Sprite](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sprite.markdown)
- Set VertexColor  to `[R:204, G:82, B:82, A:1.00]`
- Set SpriteSource enum to `CircleBordered`
- Command : [PlayGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#playgame)
- Use the `Arrow` keys to move the Player object

** ADD IMAGE **

- Command : [StopGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#stopgame)

In a moment, we'll make it possible to go to the gameplay level from the main menu, but while we're here, let's make it possible to exit to the menu from gameplay.

## Going from Gameplay to the Main Menu

Let's make it so that the `Escape` (Escape) key takes us back to the main menu. Of course, by default, this key quits a Plasma game altogether. We'll use a combination of two new components to circumvent this functionality and replace it with our own.

- Command : Add Resource
- Create a LightningScript resource using the Component template template and name it `QuitHandler`
- Update the `QuitHandler` script to the following:

<pre><code class="language-csharp" name="QuitHandler">
class QuitHandler : LightningComponent
{
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.GameSession, Events.GameRequestQuit, this.OnGameRequestQuit);
  }
  
  function OnGameRequestQuit(event : GameEvent)
  {
    event.Handled = true;
  }
}
</code></pre>

When `Escape` is pressed, the [GameRequestQuit](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/event_reference.markdown#gamerequestquit) event is dispatched to the GameSession object. If this event is not **handled**, the game exits. This component allows us to prevent this.

- Command : Add Resource
- Create a LightningScript resource using the Component template template and name it `LoadLevelOnKeystroke`
- Update the `LoadLevelOnKeystroke` script to the following:

<pre><code class="language-csharp" name="LoadLevelOnKeystroke">
class LoadLevelOnKeystroke : LightningComponent
{
  [Property]
  var Key : Keys = Keys.Escape;
  [Property]
  var LevelToLoad : Level = Level.MainMenu;
  
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(Plasma.Keyboard, Events.KeyDown, this.OnKeyDown);
  }
  
  function OnKeyDown(event : KeyboardEvent)
  {
    if (event.Key == this.Key)
      this.Space.LoadLevel(this.LevelToLoad);
  }
}
</code></pre>

This component loads the specified level when the chosen key is pressed. With these two components, we can go from the gameplay level back to the main menu.

- Select : LevelSettings object
- In the Properties Window
- Add Component : `QuitHandler`
- Add Component : `LoadLevelOnKeystroke`
- Command : [PlayGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#playgame)
- Press `Escape` while playing the `GameplayLevel` Level resource

** ADD IMAGE **

*It's now possible to go from gameplay to the main menu*

Pressing `Escape` while in the gameplay level now takes you to the main menu; pressing it again from there will quit the game.

NOTE: We've placed the `QuitHandler` component on the LevelSettings object object in the gameplay level, so that's the only level where the `Escape` key won't quit the game. To suppress Plasma's default Escape-to-quit behavior in other levels, add a `QuitHandler` to their LevelSettings object (or another object in the level). To prevent it on a broader scale still, add it to the Space object or even the GameSession object.

- Command : [StopGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#stopgame)

Now to hook up the main menu to go into the gameplay level.

# Going from the Main Menu to Gameplay

- In the `Library Window`
- Open the Library enum list menu
- Select your project's library
- Under the Level  tag
- Open the `MainMenu` Level resource
- Select : StartGameButton object
- In the `Properties Window`
- Under `LoadLevelOnClick`
- Set LevelToLoad enum to `GameplayLevel`
- Command : [PlayGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#playgame)

** ADD IMAGE **

Clicking the **Start Game** button now loads the gameplay level, from where the `Escape` key can be used to return to the main menu.

- Command : [StopGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#stopgame)

We're almost done. Next up: a credits screen.

# Creating a Credits Screen

The credits screen will be a modified copy of the main menu, so we can begin by duplicating the `MainMenu` level. Then we'll open the copy and make our changes to it.

- In the `Library Window`
- Under the Level  tag
- Right click the `MainMenu` Level resource
- Select **Duplicate** to create a copy of `MainMenu`
- Rename the `MainMenuCopy1` Level resource to `Credits`
- Open the `Credits` Level resource

The credits will be displayed in a window like the main menu's menu window, but with only one button at the bottom that will go back to the main menu.

- Select : RootWidget object
- In the `Properties Window`
- Under [UiRootWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uirootwidget.markdown)
- Set LocalColor  to `[R:64, G:25, B:51, A:1.00]`
- [Delete](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#delete) : CreditsButton object, ReturnToTitleButton object, and QuitGameButton object
- Select : MenuTitle object
- In the `Properties Window`
- Under [SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Credits`
- Select : StartGameButton object
- In the `Properties Window`
- Rename the StartGameButton object to `MenuButton`
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Under the **Layout** group
- Set SizePolicyY enum to `Fixed`
- Set the **Y** part of Size  to `40`
- Under `LoadLevelOnClick`
- Set LevelToLoad enum to `MainMenu`
- Select : ButtonText object
- In the `Properties Window`
- Under [SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Return to Main Menu`
- Set FontSize  to `16`
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `22`

Now we're going to explore a concept we haven't touched yet: giving a widget object a **size policy** of `Auto`.

- Select : MenuWindow object
- In the `Properties Window`
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Under the **Layout** group
- Set SizePolicyY enum to `Auto`

A widget object with a **layout** component, like [UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown), can resize itself when laying out its children. The `Auto` size policy causes such a layout to make itself as small as necessary to accommodate all of its fixed-sized contents, including its padding and spacing, the margins of its child widgets object, and any of those children that use the `Fixed` size policy. In the case of the credits window, it contains only two direct children, each of which is `Fixed` on the Y axis. Their Y size plus the padding and spacing of the window's layout determines the Y size of the window:


### MenuTitle object has a `Fixed` Y Size  of `41`

### MenuButton object has a `Fixed` Y Size  of `40`

###  MenuWindow object has a PaddingTop  of `4`

### MenuWindow object has a PaddingBottom  of `4`

###  MenuWindow object has a Y Spacing  of `4`

These all add up to `93`, which is exactly the height of the window.

** ADD IMAGE **

*The credits window, with its SizePolicyY enum set to `Auto`, with hierarchy for reference*

The credits will be displayed between the menu title and the button. We'll place them in a [UiStackLayout](https://github.com/zPlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/uistacklayout.markdown) that we can make by starting with the `UiSprite` archetype. We'll remove its [Sprite](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sprite.markdown) component, though, so that it's just an invisible layout area. We'll set its SizePolicyY enum to `Auto`, so that it can grow to fit every credit we add.

- In the `Library Window`
- Open the Library enum list menu
- Select the `UiWidget` library
- Under Archetype 
- `Left drag` `UiSprite` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSprite` instance between MenuTitle object and MenuButton object ** ADD IMAGE **
- In the `Properties Window`
- Rename the UiSprite object to `CreditsBlock`
- Remove Component : [ Sprite](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/sprite.markdown)
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set SizePolicyY enum to `Auto`
- Add Component : [UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)

The credits block should be a vertically stacked list, so we're using a [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown). Each element of the list is a pair of two things: a **role** (to be shown on the left) and the **people** who held that role on your game (to be shown on the right). Thus, each credit is itself a stack layout. (As we'll soon see, the list of people will also be yet another stack layout.)

- Select : CreditsBlock object
- Command : [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- In the `Properties Window`
- Rename the copy of CreditsBlock object to `CreditListing`
- Attach CreditListing object to CreditsBlock object
- Select : CreditListing object

The credits should be stacked vertically, but within each listing, the role should be listed to the left of the names of the people, so the stack direction of this new widget object needs to change.

- In the `Properties Window`
- Under [UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Set StackDirection enum to `LeftToRight`

Each credit listing will contain a role, which will be a simple text widget object, and a list of people, which will be another stack layout, like the listing itself. Before we add the role text widget object, let's duplicate the credit listing widget object and modify it to become the list of people. Afterward, we can add the role text.

- Select : CreditListing object
- Command : [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- In the `Properties Window`
- Rename the copy of CreditListing object to `ListOfPeople`
- Attach ListOfPeople object to CreditListing object
- Select : ListOfPeople object

The names of the people should be stacked vertically, and they should be centered vertically as well, just in case the name of the role takes up more vertical space than the list of people.

- In the `Properties Window`
- Under [UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Set StackDirection enum to `TopToBottom`
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Under the **Layout** group
- Set VerticalAlignment enum to `Center`

Now we'll add the role text. It'll be the first element in the credits block with a `Fixed` height, so we'll finally be able to see something! The role will be displayed on the left side of the credit listing, but it will be aligned to the right.

- In the `Library Window`
- Under Archetype 
- `Left drag` `UiSpriteText` into the `Objects Window`
- In the `Objects Window`
- `Drag and drop` the `UiSpriteText` instance on top of CreditListing object
- Reorder the children of CreditListing object so that UiSpriteText object is before ListOfPeople object
- In the `Properties Window`
- Rename the UiSpriteText object to `Role`
- Under [UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown)
- Set the **Y** part of Size  to `16`
- Under the **Layout** group
- Set SizePolicyX enum to `Flex`
- Set VerticalAlignment enum to `Center`
- Under [SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Role`
- Set TextAlign enum to `Right`

We'll fill in the actual name of the role later. First, let's put some placeholder names in the corresponding list of people. Each name will be displayed on the right side of the credit listing, but it will be aligned to the left.


- Select : Role object
- Command : [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- In the `Properties Window`
- Rename the copy of Role object to `Person`
- Attach Person object to ListOfPeople object
- Select : Person object
- Under [SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown)
- Set Text  to `Name`
- Set TextAlign enum to `Left`

** ADD IMAGE **

*A credit listing, with placeholder text, with hierarchy for reference*


The role and the person's name don't have any room between them. This can be corrected with the Spacing  property of the layout they're in.

- Select : CreditListing object
- In the `Properties Window`
- Under [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Set the **X** part of Spacing  to `16`

That looks better. Let's also duplicate the placeholder name, to see how it will look when more than one person is credited for the same role.

- Select : Person object
- Command : [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)
- Command : [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)

NOTE: Both of the above [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate) commands should be executed.

** ADD IMAGE **

*A credit listing, with multiple names for the same role, with hierarchy for reference*

That looks pretty good. Now let's duplicate the credit listing.

- Select : CreditListing object
- Command : [ Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate)

** ADD IMAGE **

*Two credit listings, with bad spacing, with hierarchy for reference*

The names run on together so that they look like they're one big list. Again, this problem can be solved by the Spacing  property.

- Select : CreditsBlock object
- In the `Properties Window`
- Under [ UiStackLayout](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uistacklayout.markdown)
- Set the **Y** part of Spacing  to `12`

** ADD IMAGE **

*Two credit listings, with good spacing, with hierarchy for reference*


That looks much better. Now we can replace all the placeholder text.

- [Duplicate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#duplicate) the CreditListing object cogs so that there are enough of them for the credits for your game
- Set the Text  properties of the [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown) components of the Role object objects to the names of the roles for your game
- Set the Text  properties of the [ SpriteText](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/spritetext.markdown) components of the Person object objects to the names of the people in the corresponding roles

If any of the names of the roles or team members in your credits extend onto multiple lines, just increase the **Y** part of the Size  property of the [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown) component of that name's widget object (say, by doubling it). Alternatively, you could also widen the whole window by increasing the **X** part of the Size  property of the [ UiWidget](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/uiwidget.markdown) component of the MenuWindow object object.

** ADD IMAGE **

*A complete credits screen, with hierarchy for reference*

# Final Connections

We're almost done! There are just a few more things to hook up, and one more quick component to make. For now, let's return to the main menu.

- In the `Library Window`
- Open the Library enum list menu
- Select your project's library
- Under the Level  tag
- Open the `MainMenu` Level resource
- Select) : CreditsButton object
- In the `Properties Window`
- Under `LoadLevelOnClick`
- Set LevelToLoad enum to `Credits`
- Select : ReturnToTitleButton object
- In the `Properties Window`
- Under `LoadLevelOnClick`
- Set LevelToLoad enum to `TitleScreen`

The quit button still has its old `LoadLevelOnClick` component from its days as a start button clone. We can remove that, and also add a new component that quits the game on click:

- Command : Add Resource
- Create a LightningScript resource using the Component template template and name it `RequestQuitOnClick`
- Update the `RequestQuitOnClick` script to the following:

<pre><code class="language-csharp" name="RequestQuitOnClick">
class RequestQuitOnClick : LightningComponent
{
  function Initialize(init : CogInitializer)
  {
    Plasma.Connect(this.Owner, Events.LeftClick, this.OnLeftClick);
  }
  
  function OnLeftClick(event : ViewportMouseEvent)
  {
    this.GameSession.RequestQuit();
  }
}
</code></pre>

- Select : QuitGameButton object
- In the `Properties Window`
- Remove Component : `LoadLevelOnClick`
- Add Component : `RequestQuitOnClick`

There's just one more thing to do: make the title screen go to the main menu.

- In the `Library Window`
- Under the Level  tag
- Open the `TitleScreen` Level resource
- Select : RootWidget object
- In the `Properties Window`
- Add Component : `LoadLevelOnClick`
- Under `LoadLevelOnClick`
- Set LevelToLoad enum to `MainMenu`
- Command : [ PlayGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#playgame)

** ADD IMAGE **

*All of the game's levels and screens are now connected*


The game is now complete. Clicking on the title screen leads to the main menu; the main menu's Start Game button leads to the gameplay level; pressing `Escape` from gameplay leads back to the main menu; clicking the main menu's Credits button leads to the credits screen; clicking the credits screen's Return to Main Menu button leads back to the main menu; clicking the main menu's Return to Title button leads back to the title screen; and finally, clicking the main menu's Quit Game button quits the game.

- Command : [ StopGame](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/command_reference.markdown#stopgame)

 

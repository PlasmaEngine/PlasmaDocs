
 #  Component Based Design
When building in the Plasma Engine your Workflow can be optimized by building things in a component based manner. What this means is that instead of attaching a single script component to a single archetype and using it to drive all the functionality of that object, your workflow can be sped up by building specific smaller actions to specific components.

When choosing how to construct a set of script components for a project it's helpful to play several games in the chosen genre and look at what commonalities they have. Using what you find you can generate a set of components you will need. 
For instance, the shooter could have used an "input component" for mouse and keyboard input, a "shoot component" to handle how shooting is done in the world, a "movement component" to handle movement through the world, a "sound component" to handle the various sounds the player will create and other varied game logic components to handle things such as health (e.g. "health component"), power ups, collisions, etc. Enemies in a shooter would probably also need a "damage on collision component" and a "special shooting component" and a "behavior component".

As with all design the correct way depends on the project. No single set of script components that will give you all your required functionality for all projects.
 

 
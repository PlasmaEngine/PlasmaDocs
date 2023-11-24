# Edge Catching

Sometimes a physics object will seem to get stuck on a smooth surface. This is often caused by an issue known as edge-catching. This issue is most common when creating a player.

In a game, the ground is often piece-wise, i.e. made of a collection of individual pieces. In this example, assume that the ground is a collection of boxes. Now a rotation locked player is implemented with a [BoxCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders/boxcollider.markdown) to move via simple velocity changes (velocity is the drawn arrow). 

![EdgeCatchingGif](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46367.gif)

Sometimes the player will stop moving even though input is setting a velocity. This behavior is caused by the seams on the ground. For an explanation of why this happens a quick physics primer is necessary.

# Physics Primer: Discrete Collision Detection
Physics engines are often implemented with discrete collision detection. This is easiest to think of as a picture flip-book where physics teleports each object from frame-to-frame. This presents a problem to physics as objects will already be overlapping by the time collision is detected. To fix collisions, physics has to approximate the best direction in which to push the objects apart. The approach taken is to find the minimum translational distance required to push the objects apart.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46368.png)

Given the above configuration, all 4 primary directions can be checked for the minimum translational distance.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46370.png)

It should be clear that pushing the box up requires less work than the other four directions.

Sometimes physics incorrectly guesses what the best distance is. This commonly happens when gravity is combined with player input and collision happens at a corner. Even though two boxes are next to each other with no seam between, physics detects collision between each box in isolation.

A step-by-step illustration is provided:

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46372.png)

First look at a movable box resting at the seam between two boxes. For this illustration the focus will be on the red box and the blue box on the right.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46374.png)

Forces for the frame are applied to the red box.  First, gravity pulls the red box down. Additionally, an input force pushes the red box to the right.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46376.png)

After updating position from forces, the physics system will see this scenario. The red box is in contact with both ground surfaces and collision needs to fix the overlap by pushing it out.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46378.png)

Each ground surface will independently determine the minimum translational distance. The left box will correctly push up. The right box will unfortunately push to the left since this requires the least movement.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46380.png)

Now physics resolves collisions and puts the red box right back where it started. Given the same forces, the red box will repeat this cycle and be stuck on this seam in the ground.

# Fixing Edge Catching

Unfortunately there is no perfect generic solution to the edge catching problem. There are two main approaches to work around the problem:

**Change your collision:** The root issue here is that a seam does exist. One way to fix this is to remove the seam by merging the surface's collision. It's near impossible to remove all seams in a game though, and it is often more practical to change the player's collision shape. Commonly, a player uses a [CapsuleCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders/capsulecollider.markdown) instead of a [BoxCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders/boxcollider.markdown) to avoid seams.

![image](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46382.png)

In the above illustration, the box on the left has a minimum translational distance that will push it to the left. The capsule however, has a minimum translational distance that is up and to the left. This will allow the capsule to move to the right a bit and escape the cycle of edge catching after a few frames. 

While this method mostly fixes edge catching, it tends to produce small bumps when crossing edges. This is because of the portion of the minimum translational distance that still points against the player's velocity.

**Use the SweptController:** Plasma provides a character controller that uses //swept collision//. Swept collision is different than discrete collision because it detects exactly when a collision happens. This prevents a player from ever colliding with an internal edge because it must first collide with the surface.

There's two issues with the swept controller.
 - It's more computationally expensive. This isn't an issue for a few number of objects, such as the player, but wouldn't be practical for every object.
 - It only works with Kinematic objects. Using the swept controller means manually translating the player and not working through velocity and forces. This swept object will no longer react to [PhysicsEffects](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/physicseffectsandregions.markdown), collision resolution won't do anything, and Joints won't affect it. For some games this may make the SweptController impractical.

# Related Materials
## Manual
- [physicstroubleshooting.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting.markdown)
- [physicsspace.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/physicsspace.markdown)
- [colliders.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders.markdown)
- [boxcollider.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders/boxcollider.markdown)
- [capsulecollider.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/colliders/capsulecollider.markdown)
- [physicseffectsandregions.markdown](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/physics/physicstroubleshooting/physicseffectsandregions.markdown)

## Reference
- [PhysicsSpace](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicsspace.markdown)
- [Collider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/collider.markdown)
- [BoxCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/boxcollider.markdown)
- [CapsuleCollider](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/capsulecollider.markdown)
- [PhysicsEffect](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/physicseffect.markdown)
- [Region](https://plasmaengine.github.io/PlasmaDocs/Plasma1/C++/code_reference/class_reference/region.markdown) 

 
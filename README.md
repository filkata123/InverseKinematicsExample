# Inverse Kinematics Example
This repo contains a simple <u>Unity<u> example which showcases IK functionality. 
It uses the "Third person" unity template, which comes with a controllable character. 

# Installation
```
1. Clone repo
2. Open Unity hub
  a. Click "Open" dropdown
  b. Select "Add project from disk"
  c. Select folder where project is cloned
  d. Open project and wait for it to load
3. If scene is empty, go to Assets -> Scenes and drag and drop the Playground.unity scene into the hierarchy -> Delete the empty scene
4. Clicking play should start the game, where the basic character can be controlled with WASD, Shift and Space.
```
  
# Functionality
The IK-enabled character is named **PlayerArmatureIK** in the Playground scene.
To enable IK functionality the following needs to be done:
  ```
  1. Hide PlayerArmature in the inspector (checkbox next to object name)
  2. Unhide the PlayerArmatureIK
  3. Click on the PlayerFollowCamera object
  4. Drag the PlayerCameraRoot child object of the PlayerArmatureIK to the "Follow" field
  ```
To test IK functionality, the character can be controlled to go over objects.
IK is used to stick the feet of the character directly to the ground beneath them, no matter the shape.
IK has also been applied to the left hand of the character.
The **LeftHand_target** object, which is a child of the Rig 1 object in **PlayerArmatureIK**, can be moved in the Scene when the game has been started manually by the user.
This target object is used as an IK effector, which will update the pose of the rest of the arm when moved.
  
# Dependencies
- **AnimationRigging** package

# Inspiration from
Rigging of hand - [Inverse Kinematics Unity Tutorial in 3 minutes](https://www.youtube.com/watch?v=TUBHvQ2XEJs)
  
Feet functionality - [REALISTIC Foot Placement Using IK in Unity](https://www.youtube.com/watch?v=rGB1ipH6DrM&t=1s)

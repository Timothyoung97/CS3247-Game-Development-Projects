# CS3247 Game Development

### Mini Project 2 Submission
- Name: Yang Shiyuan
- Matrix Number: A0214269A

### Learning Outcome
- Experiencing Blueprint System and Functionalities

### Instruction
1. Download source file from [here](https://drive.google.com/drive/folders/1Di5Mtm_udamxNq5-oyN44JOE-c1mXsSb?usp=sharing).
2. Extract the file.
3. Open using Unreal Engine by importing the extracted file.
4. Navigate to `Content/Lessons/Lesson2/MiniProject2` using Unreal Engine editor's file explorer.
5. Start evaluation.

<div style="page-break-after: always;"></div>

## HW_Lean

### Introduction
- This is a level inspired by the game "Portal". 
- When pressed on play in the Unreal Engine editor, player will be able to see a portal that leads to another location in the same map.
- Given that we have no access to VR devices, the portal serves as a good medium to provide the experience of leaning in. 
- The player will be able to lean in and see the scene that is beyond the other portal.
- In addition, player is able to step through the portal and enter another location in the map.
    
    <img src="public\HW_Lean\Screenshot 2022-02-03 030750.png" width=600/>
    <img src="public\HW_Lean\Screenshot 2022-02-03 030945.png" width=600/>

### Implementation
- This level is designed using the existing template of `MyRoom.umap` found in `Lesson 1`, with other existing assets found in VARLAB.
- In `HW_Lean.umap`, the main scripting happens in the `Level Blueprint`.
- In there, you will find:
  - `Portal 1 Teleport` and `Portal 2 Teleport`:

    <img src="public\HW_Lean\Screenshot 2022-02-03 031034.png" width=600/>
    <img src="public\HW_Lean\Screenshot 2022-02-03 031054.png" width=600/>

    - These blueprint mappings are mainly responsible for the teleportation mechanism, where the player gets teleported to another portal when in contact with the portal.
  - `portal screen cast 1` and `portal screen cast 1`:

    <img src="public\HW_Lean\Screenshot 2022-02-03 031202.png" width=600/>
    <img src="public\HW_Lean\Screenshot 2022-02-03 031253.png" width=600/>

    - These blueprint mappings are mainly responsible for the screencasting mechanism, where the player is able to see the perceived view of the other portal.

<div style="page-break-after: always;"></div>

## HW_Dip

### Introduction
- This is a simple level designed to provide the experience of dodging.
- When pressed on play in the Unreal Engine editor, player will be able to see multiple swords moving in front of the player. 
- Given that we have no access to VR devices, these moving swords are expected to motivate the player to dodge against them while trying to reach the goal ball (in orange). 

    <img src="public\HW_Dip\Screenshot 2022-02-03 031347.png" width=600/>

### Implementation
- This level is designed using the existing template of `FirstPerson.umap` in `Lesson 4`, with other existing assets found in VARLAB.
- In `HW_Dip.umap`, the main scripting happens in the `Sword` asset's `Construction Script` and `Level Blueprint`.
- In there, you will find:
  - `Sword Movement`:
  
    <img src="public\HW_Dip\Screenshot 2022-02-03 031415.png" width=600/>

    - Responsible for moving the static mesh to and fro designated point A and B.
  - `Sword Rotate`:

    <img src="public\HW_Dip\Screenshot 2022-02-04 142950.png" widht=600/>
    
    - Responsible for the rotation of the sword.

<div style="page-break-after: always;"></div>

## HW_Left

### Introduction
- This is a simple platformer level designed to provide the experience of movement within the game.
- When pressed on play in the Unreal Engine editor and Key `T` once in-game, player is able to control the 3D Humanoid and is able to see an obstacle course in front of him.
  - Control:
    - `W` = move forward
    - `A` = move left
    - `S` = move back
    - `D` = move right
    - `Space` = jump
- Given that we have no access to VR devices, these moving obstacles placed in the map is expected to motivate the player to look left/right/up/down to avoid the obstacles and move up the spiral staircase for the goal ball.

    <img src="public\HW_Left\Screenshot 2022-02-04 212421.png" width=600/>

### Implementation
- This level incorporate the imported asset of `ThirdPersonCharacter` from the Unreal Engine Tutorial.
- In `HW_Left.umap`, the main scripting happens in the `Level Blueprint` and `Blueprint` in `Disappearing Platform`.
- In there, you will find:
  - `Rotate Cube` in `Level Blueprint`:
  
    <img src="public\HW_Left\Screenshot 2022-02-03 031544.png" width=600/>

    - Responsible for the movement of the gray colored long cuboid found in front of the `ThirdPersonCharacter` when the game starts.
  - `Press "T" to switch control` in `Level Blueprint`:

    <img src="public\HW_Left\Screenshot 2022-02-03 031555.png" width=600/>

    - Responsible for switching the camera view and control from the default start-up option to the `ThirdPersonCharacter`.
  - `Blueprint` in `Disappearing Platform`:

    <img src="public\HW_Left\Screenshot 2022-02-04 212519.png" width=600/>

    - Responsible for the disappearing and reappearing mechanics of the platform
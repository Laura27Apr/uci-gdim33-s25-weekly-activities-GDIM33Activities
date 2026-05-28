# GDIM 33 In-Class Activities

## W1
### Activity 1
[Inspiration Board](https://docs.google.com/drawings/d/1sfnbYr2Jj6Pp-3PbAsxMVjZrqqeDOqv-UXVW9WTSq20/edit?usp=sharing)

1. I think the patterns emerging from my inspiration sources are the fusion of reality and fantasy, which creates an atmosphere reminiscent of a "dark fairy tale." And I think they convey a sense of contrast: these sources may seem gentle and calm, but they conceal an underlying atmosphere of oppression and a touch of the uncanny. I would like to do a visual novel, and based on those inspiration sources, I think I may not make the results immediately revealed but gradually shift. And there will be one main NPC who has a companionship with the player.


2. My tablemate is interested in building a 3D survival horror game. And it takes place at a lab or an office, and in that place, there will be experiments about making animals into monsters. And those monsters will chase you. I think we do not have much personal style and interests since she focuses more on game mechanics while I focus more on the story.


3. I do not think his taste is similar to mine since I prefer games that tell stories more, while he prefers action games like FPS.

### Activity 2
<img width="960" height="720" alt="Breakdown" src="https://github.com/user-attachments/assets/4950b1e1-9bd2-4416-9a1f-23b6f1d2d594" />



## W3
### Activity 1
<img width="1719" height="718" alt="Vertical_Slice_Breakdown" src="https://github.com/user-attachments/assets/90b663c6-7b78-4031-a556-6146e0df2afa" />


### Activity 2
1. I think saving the event name as Scene variable can make different graphs share the same event name instead of writing the name again and again. And if you want to change the name after you just need to change the name of Scene variable and you do not need to check every graph which may contain that event. It makes all the graphs more organized.


2. I think this can help you identify which graph is causing the problem in a very intuitive way. By adding different debug logs to different graphs, I can narrow down the issue step by step. For example, I can determine whether a click is not registering, an event is not being passed to the GameController, or the transition itself is not being triggered. This allows you to identify the problem early on rather than deleting elements one by one and retesting blindly.


3. Set Cursor Lock State is relevant to my vertical slice. In my vertical slice, I want the player to be unable to see the cursor while moving, but to be able to see it when selecting dialogue options or reading documents. Therefore, this feature is very useful to me. Additionally, I find controlling the cursor via visual scripting to be more intuitive than using C#.


4. This is also relevant to my Vertical Slice since in my game there will be 3 different states for the player, which is Exploring, Talking and Reading. I will use it to control the cursor state and player's movement. The player will switch between these states based on input, such as pressing the F key or ESC. 



## W4
### Activity 1
#### Playtesting Preparation
Playable:
	1. The player should be able to move with WASD and the cursor to look around;
	2. The fox will change its state after the player reaches to it, from alert to the calm;
	3. The player can click to start the dialogue to the fox.

Goal:
	1. Is the movement of the player good?
	2. Is the size of the dialogue box ok?
	3. Is the camera position high?

#### Playtest Team
Bilal Payton, Kai Castilliano, Alejandra Perez

#### Playtest Notes
My game appears to be to big to run on the itch and I tried to change the asset max texture size to max 64 but it still shows:
<img width="1920" height="741" alt="屏幕截图 2026-04-22 204851" src="https://github.com/user-attachments/assets/33964157-4c36-44df-bc96-cf7db5c9ba18" />


Therefore I tested in the Unity. TT
1. Make the Cursor have different states will be better;
2. Of course lock the player movement when there is dialogue going on.


### Activity 2
1. A writer could add more dialogue to this setup without writing any code, since in this setup the dialogue is saved into the ScriptableObject instead of saving into the code. A writer just needs to add more DialogueNodes and put the lines and the replies to write the dialogues.


2. I do not think there is a clear number of dialogue nodes that the writer could create without writing any code since different dialogue nodes exist individually, and we just need to make sure they are connected correctly to add as much dialogue nodes as the writer wants.


3. I think Regenerate Nodes acts like a refresh button. It allows the system to regenerate different events or other nodes based on the current data. This is because when I edit content in C#, it might not sync automatically. In such cases, Regenerate Nodes ensures that the dialog structure I see and use matches the content I have just written.


## W5
### Activity 1
1. Make the NPC follow the player using the Navmesh.
	1. Create and bake the NavMesh. Check whether the blue mesh covers the expected areas by eyeing it.
	2. Create a target position with an empty GameObject in the scene. Code the NPC to move toward it in Start() using SetDestination(). This tests the NavMesh and the basic usage of NavMeshAgent on the NPC.
	3. Replace the target position with the Player’s Transform. Move the NPC to continuously update its movement target to the player. Run the game to test.
2. Make the NPC follow the player only after the dialogue ends and the Player is in the Explore state.
	1. Connect the NPC movement to the player state machine. Only allow the NPC to move when the player is in the Explore state. Use Debug.Log to confirm when the player enters the Explore state, and the NPC is allowed to move.
	2. Trigger the following behavior of the NPC after dialogue ends. When dialogue ends, the player returns to the Explore state, and only then does the NPC start following the Player. Run the game to test.
	3. Pause the NPC’s movement when entering the Dialogue State of the NPC. Run the game to test.
3. Trigger the NPC follow behavior when there is a certain distance between the NPC and the Player.
	1. Add a distance check to control when the NPC should start to follow the player. Use Debug.Log to print the distance value and confirm that the NPC follow behavior only triggers when the distance condition is met.


### Activity 2
First, I have created and baked my NavMesh. Then I coded a script which let the NPC came to the player once the game start. And once the player left the initial place and there is certain distance between the player and the NPC, the NPC will start follow the player.


## W6
### Activity 1
- I have added NPC follow behavior after the first round of dialogue which results in NPC following the player when the player is exploring the environment around; I have also added an interaction GameObject which the player can press F to read and press ESC to exit the read mode.

- [Playtest 2](https://laura27apr.itch.io/playtest2-gdim33)

- Goals:
1. Test if the dialogue branches really affect player's exploration of the environment;
2. Test if the reading UI works well, is it clear?
3. Check if more guiding UI elements are needed.

- Notes:
1. Absolutely lock the cursor when the player is not in the dialogue;
2. Add collider to the big assets in the game to make sure that the player and the NPC does not go through it;
3. Add the walking animation for the NPC;
4. Add a new scene before the real game begin to explain the background story.

### Activity 2
1. I think this because when we are multiplying the numbers which are greater than 0 but less than one, usually the results we get will get smaller and smaller. And in the RGB channels, as the number of the RGB get less, the color gets darker and less saturated. This is the reason that Multiply setting of the Blend node makes the resulting color darker and less saturated than the input colors.

2. The resulting value will be more translucent since the values in the Alpha are also from 0.0 to 1.0. And when we are multiplying, the values will get smaller. And in the Alpha, as the value grows from 0 to 1, the transparency also grows from more translucent to more translucent. Therefore, the resulting value will be more translucent.

3. I think the UV values are from the assets (models) themselves. Each vertex of the assets has its UV coordinates, which could tell the shader.

4. Kind of? Because through that I know how to control the color through numbers, which I may also use when I am coding. I can easily adjust the color detailedly through changing the numbers.


## W7
1. The data for the Vertex Color node comes from the Shiba model itself. Each vertex in the mesh assets in the Shiba model contains a Position, Normal, Tangent, Color, and UV.
2. This is because the vertex data interpolated (blended) between the fragments in the fragment shader. The GPU will blend colors based on the distance between the distance of each fragment and different vertices.
3. Vertex color is less detailed because the color data is only stored at the vertices. And if we do not have enough vertices, the color will seem rough. Vertex color can be useful for simple coloring and debug purposes.
4. I think the colors near the shiba’s back thigh look wrong since it is different from the colors on that part.
5. I think we can test UV data. Since UV is commonly hard to observe, and is we use debug shader makes it easier to observe the problem.
6. At the beginning, the normal direction and the light direction are opposite. And if the two directions are opposite, we have a negative result value, which results in the reverse lighting.
7. The additive mode can add the color of the object being drawn to the colors already on the screen, which makes the bright area look more obvious.


## W8
### Activity 1
- I have added more interactable items and added readings for them. Also, I have added a beginning scene for my game which illustrates my game's background story.

- [Playtest 3](https://laura27apr.itch.io/playtest3-gdim33)

- Goals:
1. Test if there is enough content right now for the game;
2. Test if the background story gives instruction for the player;
3. Check if there is more dialogue content needed;

- Notes:
1. It may be better to add more clues here for the player to explore;
2. Add background music and sound effects;
3. Fix the default dialogue.

### Activity 2
2C:


1. FullScreenPassRendererFeature. I think other than the name being kinda obvious, I can tell because the events happens before this pass do not contain the red texture I added, it is just the normal scene.
2. When the Lerp value is set to 0.5, we can see a little bit of the texture. When the Lerp value is set to 0, we cannot see the texture at all. When the Lerp value is set to 1, we can see that the texture is completely shown on the screen.
3. Because Lerp will use the value to blend the texture and the original scene. The closer the value is to 0, the more it leans toward the original image. The closer the value is to 1, the more it leans toward the effect.
4. From the graph, we can see that the sin(time) contains value from -1 to 1, while (sin(time)+1)/2 contains value from 0 to 1, which means (sin(time)+1)/2 does not contain negative values. And for the Lerp, it is only supposed to have input values from 0 -1. Therefore, the negative value will result in the bright stage.


## W9
### Activity 1
Minecraft:
	1. Cube Outline effect:
		- When a player hovers cursor over a block there is an outline over it to indicate to the players what block they are going to either mine/place something on. 
		- We think that this effect is a renderer feature that is applied to certain objects.
		- This game effect is activated when the cursor is pointing to the specific game objects and it is deactivated when the cursor is not over the object. 
	2. Teleportation effect (Nether):
		- Full-screen post-processing effect 
		- Maybe it has a timer to activate and deactivate while the other world(Nether) loads.
	3. Effect of attacking something:
		- When player hits something living (mob, another player) they turn red for a brief moment  
		- Material change? 
		- An effect in an individual object's material
		- Set a timer to control red effect using Time.deltaTime




### Activity 2

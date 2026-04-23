# GDIM 33 In-Class Activities

## W1
### Activity 1
[Inspiration Board](https://docs.google.com/drawings/d/1sfnbYr2Jj6Pp-3PbAsxMVjZrqqeDOqv-UXVW9WTSq20/edit?usp=sharing)

1. I think the patterns emerging from my inspiration sources are the fusion of reality and fantasy, which creates an atmosphere reminiscent of a "dark fairy tale." And I think they convey a sense of contrast: these sources may seem gentle and calm, but they conceal an underlying atmosphere of oppression and a touch of the uncanny. I would like to do a visual novel, and based on those inspiration sources, I think I may not make the results immediately revealed but gradually shift. And there will be one main NPC who has a companionship with the player.


2. My tablemate is interested in building a 3D survival horror game. And it takes place at a lab or an office, and in that place, there will be experiments about making animals into monsters. And those monsters will chase you. I think we do not have much personal style and interests since she focuses more on game mechanics while I focus more on the story.


3. I do not think his taste is similar to mine since I prefer games that tell stories more, while he prefers action games like FPS.

### Activity 2
<img width="960" height="720" alt="Breakdown" src="https://github.com/user-attachments/assets/4950b1e1-9bd2-4416-9a1f-23b6f1d2d594" />



## W2
### Activity 1
<img width="1719" height="718" alt="Vertical_Slice_Breakdown" src="https://github.com/user-attachments/assets/90b663c6-7b78-4031-a556-6146e0df2afa" />


### Activity 2
1. I think saving the event name as Scene variable can make different graphs share the same event name instead of writing the name again and again. And if you want to change the name after you just need to change the name of Scene variable and you do not need to check every graph which may contain that event. It makes all the graphs more organized.


2. I think this can help you identify which graph is causing the problem in a very intuitive way. By adding different debug logs to different graphs, I can narrow down the issue step by step. For example, I can determine whether a click is not registering, an event is not being passed to the GameController, or the transition itself is not being triggered. This allows you to identify the problem early on rather than deleting elements one by one and retesting blindly.


3. Set Cursor Lock State is relevant to my vertical slice. In my vertical slice, I want the player to be unable to see the cursor while moving, but to be able to see it when selecting dialogue options or reading documents. Therefore, this feature is very useful to me. Additionally, I find controlling the cursor via visual scripting to be more intuitive than using C#.


4. This is also relevant to my Vertical Slice since in my game there will be 3 different states for the player, which is Exploring, Talking and Reading. I will use it to control the cursor state and player's movement. The player will switch between these states based on input, such as pressing the F key or ESC. 



## W3
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


<<<<<<< HEAD
3. I think "Regenerate Nodes acts like a refresh button. It allows the system to regenerate different events or other nodes based on the current data. This is because when I edit content in C#, it might not sync automatically. In such cases, ¡°Regenerate Nodes¡± ensures that the dialog structure I see and use matches the content I have just written.
=======
3. I think Â¡Â°Regenerate NodesÂ¡Â± acts like a refresh button. It allows the system to regenerate different events or other nodes based on the current data. This is because when I edit content in C#, it might not sync automatically. In such cases, Â¡Â°Regenerate NodesÂ¡Â± ensures that the dialog structure I see and use matches the content IÂ¡Â¯ve just written.
>>>>>>> 0962af91f77ac4f3f7c9cab89c6ad82c9e0c22e1


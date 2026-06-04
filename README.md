# GDIM 33 In-Class Activities
## W1
### Activity 1
[Pinterest Board Link](https://www.pinterest.com/personalhernandez17/gdim33-vertical-slice/)

1. I've noticed that I have gravitated towards a third-person survival horror game, with gunplay similar to TLOU and RE. While I hate anything horror related, I was having fomo because of the release of RE9 and decided to play it at my friends house and actually really enjoyed it, despite my disdain for the genre. As a result, RE has been on my mind a lot and I think it would be a fun gameplay loop to replicate to the best of my ability. Also I watched like half of Cowboy Bepop, and I like the idea of a horror game taking place in a retrofuturistic universe. Thematically I want the game to allude to imperialism. The monster (from another planet) will be a steel figure to personify technological advancements in weaponry. The chracter's gun will do little damage to the monster. The player will be able to kill the monster by crafting a bullet out of chunks dropped by steel monster. 
2. Most of my table mates were also interested in making a survival horror game, which I am looking forward to as we will all get to see our projects grow together. Celo drew inspiration from Borderland's artstyle, which was interesting because I also really like cell-shading.
3. Eric our TA said his favorite genre is FPS games, which I enjoy from time to time as well. An fps game I would definitely recommend is The Finals, which I play with one of my friends occasionally. 


### Activity 2
<img width="1620" height="1202" alt="image" src="https://github.com/user-attachments/assets/0d1f6318-cb0c-4bc7-b585-1b23c43ac828" />



## W3
### Activity 1
<img width="960" height="720" alt="Untitled drawing (2)" src="https://github.com/user-attachments/assets/2841620f-6c35-4ea0-be0a-beb1e3dc8fa7" />

### Activity 2
1. It is advantageous to use a scene variable for the event because we can then fire the event from a seperate object.

2. Using a debug.log node helped me to detect if the event transitioning from explore to dialogue was firing. We had struggled to fire the event due to the fact that we were referencing the event incorrectly from the other script machine. We were able to find the source of the area because my "Hi" message wasn't appearing in the console.

3. Yes it is because my game is going to run in a third person over the shoulder perspective, which means that the mouse will need to be able to control the camera within the confines of the scene window.

4. Yes because in my vertical slice both the player and the monster will have multiple states. For example, the monster will be able to wander, pursue, and attack.

## W4
### Activity 1
1. Movement and Aim down sights.
2. Playtesting goals: how do they feel about the slow down effect, how do they feel about the level
3. Notes: The movement speed is a nice touch, the world looks cool, gunplay needs to be added ASAP

#### Playtesters 
Kai M, Kai L, Marcelo T, Nathan H

### Activity 2
1. Yes because the scriptable objects allow writers to add dialogue nodes through the inspector.
2. The writers could conitinously add nodes I believe, without writing code.
3. It provides nodes for visual scripting that are not necessarily readily available within the scene. Some may come from imported packages or may be created by the player; the regenerate node button implements all of them inot the node library.

## W5
### Activity 1
NavMesh Monster
1. Make npc move towards player using NavMesh
   
   a) create + bake NavMesh
   
   b) make NPC move towards player
   
   c) make NPC pursue on every frame
   
2. NPC controller by sightlines
   
   a) draw raycast using gizmos
   
   b) make NPC stop chasing player when out of sight
### Activity 2
Completed Step 1, completed step 2a.


## W6
### Activity 1

Whats New?: NavMesh monster mechanics

Playtest Goal: answer these questions

How does the new sensitivity feel?

Should the monster be slower?

How hard should the monster be easier to escape from?\

Notes: the sensitivity is too high, the monster should be easier to slow down, the escapability factor is okay.

### Activity 2

1. The RGB values are factors of less than 1, which decreases the saturation and brightenss, as multiplying by a decimal value decreases the product.

2. The result would be a more transluscent figure because multiply decreases the value when combining two colors. Since alpha handles the transparancy of materials, multiply will make the object more opaque

3. The shader gets the UV values from the nodes itself, as the UV graph is what determines the transform of each vertice within the texture, aligning it with a game object. Without the UV0 node being created, the sample texture wouldn't be able to properly render the position of each vertice.

4. i like color and i like math

[itch build](https://nathannnhernandez.itch.io/hiddeninhavenbuild2)


## W7
For our vertex color shader in step (2), where did the data for the Vertex Color node come from?
   
   Most of the nodes contain data from the original mesh.


Since vertex color is stored as data in each vertex of the mesh, why is the color on our shiba from step (3) blended at the edges of different regions of color?
   
   The normal debug shader uses xyz components of surface normals to apply the texture.


Why is the shiba from step (3), which is colored with vertex color, less detailed than the shiba we rendered with a texture in last week’s activity? Given that vertex color generally results in a less detailed color application than applying a texture, what can you imagine vertex color is useful for?
   
   The Shiba is less detailed because vertex colors are less detailed than textures. This can be useful for optimization as they are less demanding.


Based on the color of the shiba in step (3), does anything look wrong with the mesh’s vertex normals?
   
   On the hip of the Shiba, there is a visual blemish that does not fit in the context of the vertex shader.


We used the color output of a shader to visualize a mesh’s vertex normal values in step (4). Name one other piece of vertex data (or any kind of data) you can imagine testing with a debug shader like this, and describe why that might be useful.
   
   Testing lighting with a debug shader can be useful, due to the impact the direction of surface normals has on the visual product of a shader graph.


Why is there an error in the lighting in step (4) on the back of the Shiba?
   
   The blemish on the back of the Shiba results from the fact that the surface normal is negative relative to the rest of the Shiba.


Why do you think we set the Blend Mode to Additive for the fire effect in Step (5)?
   
   The formula inherent to additive blending ensures that the colors will shine brighter than alpha blending, due to the fact that alpha blending multiplies by a decimal factor

## W8
### Activity 1
The main issue with my game was that the level wasn't intuitive enough. With all of my mechanics now implemented, I can start designing my level and creating the setpieces I intend to add into the game. I also want to add lore drops, which would add more context as to what the player needs to do in order to win.   

What has changed: Since milestone 2, the only thing that has changed in my game was my monster. I imported a robotic looking creature from an animation site and gave him unique animations for movement. I need to add an attack animation for sure tho.

### Activity 2
Open the Frame Debugger window under Windows >Analysis > Frame Debugger. What's the name of the pass associated with the post-processing effect we created? Other than the name being kinda obvious, how can you tell?
I think it is uberpost. You can tell by unfolding the render post processing effects tab, then navigating to uberpost process and checking for the pass.

What does the screen look like if the Lerp value is set to 0.5? What about 0? What about 1?
The lower the value, the more opaque the visual effect.

WHY does the screen look like that based on those different Lerp values?
The third value of the lerp node is th alpha valy\e which determines the opacity.

Why does our algorithm for the Lerp amount use (sin(time)+1)/2 instead of just sin(time)? (see instructions for hints)
The range of the sin function is between -1 and 1, however we need values between 0 and 1.

## W9
### Activity 1
Mario Kart VFX Examples

Effect 1: Mario Kart Ink Debuff

This is a full-screen post-processing effect applied to the entire camera 
The shader involves applying temporary moving inkblot textures to the camera after the player gets attacked by a squid powerup
I might activate the effect by enabling an entire post-processing effect and then using methods to instantiate inkblots at random coordinates. Once created, the inkblot shader graph will handle its shape and movement. 

Effect 2: Mario Kart Star Power Up Cart Effect

Individual Object’s Material
This would be activated when players use a star power up
I believe that this involves multiplying the rainbow effect on top of the model of the player and their cart kind of like the shiba activity but instead of replacing the model it combines them. The rainbow effect would likely be drawn from a pre-made gradient texture. 
### Activity 2
<img width="1569" height="992" alt="image" src="https://github.com/user-attachments/assets/fdcda786-df50-4501-9efa-7f78a25a6d10" />

Created the material + graph for the damage vignette effect, just need to trigger on hit now

## W10 :)
### Activity 1
- Feedback on level design

- Feedback on difficulty

- Feedback on audio

- Feedback on VFX

- Response: add lore early on, vfx looks cool but doesnt function right on itch, balancing is good but add sensitivity slider for preference

### Activity 2
1. Identify game: mechanics, systems, aesthetics, narrative, etc
2. Breakdown game systems using bubble charts that conect each system
3. Create a macro/burndown chart for your project's scope
4. Focus on scalability based on game identification: use prefabs, serialized fields, scriptable objects, singletons, parent classes, etc
5. Playtest frequently (at least every other week): new and returning players
6. Create playtest goals + take notes

As for a games scope, if your vertical slice is fat, it can be hard to make it tall. Breaking down the core mechanics of your game can make it much easier to recognize when your slice is getting too fat.

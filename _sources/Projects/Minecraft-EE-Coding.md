# Coding with Minecraft

Added: 20210727-1732

#STEMProjectTopics #ICTCourse #Virtual-Robotics 

- [Projects](Projects.md)
- [STEM09-ADST-Survey](STEM09-ADST-Survey.md)
- [Minecraft-EE-Coding](Minecraft-EE-Coding.md)
- [MinecraftCoding - Google Drive](https://drive.google.com/drive/folders/1bwaL67pUBaWmqVNUTg7qiyGatni8RmKz?usp=sharing)
- [P2-MinecraftEE](https://vsbworld-my.sharepoint.com/:f:/r/personal/cjanze_vsb_bc_ca/Documents/STEM09/P2-MinecraftEE?csf=1&web=1&e=Npta8a)  110 Resources to vet
- see: [ICT-Elements-of-Code](ICT-Elements-of-Code.md)
- see: [ICT-Rubric](ICT-Rubric.md)

## Survey3 Coding with Minecraft EE

[P2 Coding with Minecraft EE](https://teams.microsoft.com/l/message/19:e9584c19ad944e3f9bf3c26442cecc4d@thread.tacv2/1622567705903?tenantId=0b8a2e58-7b30-4a08-bab7-d75559e0e3a5&amp;groupId=70cd545c-5227-41de-af89-f32585f43143&amp;parentMessageId=1622567705903&amp;teamName=STEM)

### Coding with Agents in Minecraft
- see [Making a Maze](https://docs.google.com/document/d/1k8-cQ2vtIL22OM1DHMGFJtj68hpWVnJPHhLX0NEZW2Y/edit?usp=sharing)
- see [Maze Pathfinding](https://docs.google.com/document/d/18qdeVd0Sk1z_S83BnzWM6ktu3qk3KsX8OzVvVpYmDKc/edit?usp=sharing)

#### Getting Started
- Minecraft EE is installed on the computers (remember to log off)
- see [Education Edition Setup for MakeCode](https://docs.google.com/document/d/1ZCUny_fF8sOX0ljlOd-Or5QI08Rz7M3d2qj5Acw37FE/edit?usp=sharing) for how to start Makecode Tutorials from within Minecraft EE
	- Complete Chicken Rain, 1000TNT and Agent Pyramid
- see [Minecraft for Windows 10 Setup for MakeCode](https://docs.google.com/document/d/1MqFsD05GF0kpK3EC4P0vVX2SFLoLYM7wzIM1U4M4UBo/edit?usp=sharing) to use Code Connection and code at home with your personal version of Minecraft for Windows 10.
- [https://educommunity.minecraft.net/hc/en-us/articles/360047555391-Importing-and-Exporting-Your-Worlds-](https://educommunity.minecraft.net/hc/en-us/articles/360047555391-Importing-and-Exporting-Your-Worlds-) 


## Making a Maze
- [minecraft.makecode.com /courses/csintro/ai/activity-1](https://minecraft.makecode.com/courses/csintro/ai/activity-1)

---

Learning how to read and write go hand in hand. To become better at writing code yourself, it is good practice to read other people’s programs. Try to read and understand how they work. For this activity, instead of writing code, you will explore an existing program for creating a maze. 

### Generate a maze from existing code
1.  Launch Minecraft and create a new Flat world in creative mode    

![Grass world template](https://lh5.googleusercontent.com/MUzo0BoTAdJWFja_ovhf4r_UnXtr_wnrMBN1K3MkeEa_Cb_JxCV_c0LcJcubnqfsm6HcpCW9T08ddyUbMd7lKvGW2F0pJAhGcHID51UyE1nI8ds787hGY_I2-2oXrP3JZ_-bS22N) 

You can use the Blocks of Grass template in Minecraft: Education Edition

![Minecraft flat world setting](https://lh3.googleusercontent.com/b-2SNcMJflZ_N4KoqTdQFgVM7KPHAdQ0K7zlk5gxXutIpM1DRareDYgLwoRyewvSWunoaVdBzB0FsU92ugbKhJMSA4r-NXvH2Cnn0TZ3WbMAVLxMi6cAFKeqrZ1-r7-BtJ69oZ9v)

  1. Set the game mode to Creative, and World Type to Flat.
  2. Open MakeCode in the Code Connection app
  3. Select the Import button in MakeCode
    

![Code Connection homepage](https://lh4.googleusercontent.com/2Cs3EzlzuSlxzlboU_4qso-HNxFI8MbroOppS6KmzfiXrL_fYwKZEdtCVHQEkZetVMCL_X8TT8T0oWDdUMBeWXWMu8FOHnIjFk1XwJ2Y5RGpqX_-gJwSRj_xPDkXn_BmBQeL7-qA)

1.  Select the Import URL card
    

![Import URL button](https://lh3.googleusercontent.com/sBuzSuz_Gr-hmC4ObXfh8IMNCqR9qHv0NUJzMy0Q9Yr5c7Gje0sP9us6_gmMtH0fyL4J5lvqdYfOhQgCYhyiX1eYBPOfDCwr4vGIRj2aVmjXEW0eDC68ByhjxMwWBmbe27UC7Izj)

-   Paste this URL in the text box and import the code: [https://makecode.com/_9EP0Vt048K0U](https://makecode.com/_9EP0Vt048K0U)
    

The code for this Maze Generation program is a bit more complex and developed in JavaScript. Basically, the Maze on chat command creates a 10 x 10 block of stone around the Player’s location. The Dig function will instruct the agent to dig out the maze from this block of stone. If the agent breaks through a wall in the maze, it will patch it up using the blocks in the agent’s inventory. The Shuffle function will ‘shuffle’ the directions that the agent will try digging in, to create a random maze pattern. You can preview the chat command “maze” in the blocks below:

The agent will need materials to patch holes it makes in the maze. Because the agent is “learning” as it goes, it may accidentally break a block of the maze wall only to later realize we need that block. Thus, the agent then patches the hole it made by mistake. You can give the agent some wood to patch the holes.

-   Give the agent some oak wood planks in its inventory, in the upper left inventory slot.
    

To give your agent something to place, go over to your agent and right-click on it. Move some blocks from your player’s inventory to your agent’s inventory like shown in the picture below. The blocks must be put in that upper left-hand box or the agent will place nothing.

![Agent's inventory](https://lh5.googleusercontent.com/EuuP6IMOpRxNJXK0MrQogZxF3Wgye4AFwtc8UX3cthTEGS5g430rm5y2MHiq4EzdwzNsByP2KJ6YugpD7iX09ujMeUCbT8jCrbw0dLl2-whNoqnHFW30TuUhYzIG8ACPRh88ZfZQ)

Let’s try out the program!

-   Type the command “maze” in the chat window to see the program run. Double tap the space bar and fly up to get a bird’s-eye view of the agent while it works. It is important to stay clear while it builds the maze.
    

### Maze pseudocode

Here is the maze solution in pseudocode:
-   Shuffle the array:
-   Create an array of three directions
-   Randomize their order
-   For each value in the array:
	- If it's left,
		-  turn left
	- If it's right,
		-  turn right
	-  If there's a wall in front of us (empty on the other side),
		-  preserve the wall
	-  If there's no wall in front of us,
		-  dig a path forward (recursively by calling the same function "dig" again)
	-  Back up 2 spaces
	-  Turn back to original direction
    
The main idea is that the agent will continue to carve an erratic path through the solid block until it reaches a blank space, trying not to destroy walls between passages. Notice that at the very end it calls the same function again in order to restart the maze carving. This is a special form of iteration known as recursion.

  
### Build the starting and ending locations

For the next activity, the agent will need to know when it has successfully completed the maze. In activity 2, you will be creating some code to get the agent to navigate the maze successfully. To get set up for the next activity, you will need to prepare the starting and ending areas of the maze.

You will need to equip the player with a diamond pickaxe and redstone block. The pickaxe is to destroy the stone for the starting point and ending point. The redstone will mark the ending point. Open Terminal using ‘/‘, then type the give command to equip the player with a diamond pickaxe and a block of redstone.

~~~
/give @s diamond_pickaxe
/give @s redstone_block
~~~

Now all you need to do is build a starting and ending point.
  1. Decide a starting point and an ending point. Most likely these will be on opposite ends of the maze.
  2. Destroy a block at the starting point.
  3. Destroy a block at the ending point. Place a redstone block underneath the ending point.    

![Destroy area for ending location](https://lh4.googleusercontent.com/z0zzGvjGz-we-8KX36je8BdsB_PSONkKOR76YsYL83I2Qafsvy4AnqdOhjP9xTDuEPfVsRMKBfnKJx6N4Y16vWVBKokcFNKgaBsUGR7QCeB7vwuCSoplH6FGdHB5DQHM8cCcpkL8)

After destroying the grass block that marks the ending location, place a redstone block in the dirt.

![Place redstone block at ending location](https://lh4.googleusercontent.com/RwJ_KFz4K9zp84h7txNHaMtQjAUT4LGdCg03wBwONBeV2LWQKqTuLpqCaCczKPWJLxeM6Ss28VjeKnTgJObXNIq91b-z0Vr4iqeb6sBgKOY8NwmZjrfQ-JH4uAXXS4teZb-IJ6MC)

In the next activity, Maze Pathfinding, you’ll have the agent stop when it detects redstone under its feet. This is how you will know it has completed the maze!

![Complete Maze Setup](https://lh4.googleusercontent.com/GKls63mcGg_wV2QZLIgjBlZv4xO8iZen6YN66cXBNWQURxKiUycEvJFvlT_wgbc_YUDN7sq3Ng4Qcxi5egJbjqvelr_Fp-7XwLWwzEWuKJ48CG3RAWGiLAsx9huKrxzLqsFeTLqK)

### Activity reflection

#### Questions
1.  Describe what the fill block does.
2.  Why do we Place a block of Air at ~0 ~0 ~0?
3.  Why do you think we set agent destroy obstacles to false?
4.  What is the difference between the two Teleport commands?    

Maze generation algorithms are a popular programming exercise because there are as many different approaches as there are types of mazes! It’s also fun to see the maze as it’s being created. The maze generation routine we are using here is adapted from an algorithm called “recursive backtracking”.

### Challenge

Let’s change some things to make our own different and unique situations!

#### Challenge 1 - Give the Player a Perch for the Bird’s-Eye View

A minor issue is that we don’t have anything to stand on and watch the agent build if we choose to. It would be nice to be teleported up to a block when the maze starts. We can then watch comfortably.

##### Tasks
1. Add a block for the player to stand on
2. Teleport the player up to that block.    

![Perch for Better View 1](https://lh6.googleusercontent.com/SvBpWtmu0OtTros_qLAa0uIpCb0DprOA64oMmtPR9Fv_iSkuXydQnuSxXr6i6RXfRhEsMOGhyurVmYsUvYmIlWioTWknjx6Fq83ZlIzaVHbfbTqjt9kL7DwdMOtCcbnDIPtcFa-w)

![Perch for Better View 2](https://lh6.googleusercontent.com/C14GG3peFLd058afdZWAFgziDDkcAMeuL8dtKH5QKvrmum95R5RFPLGA2Uv-w2I9gp3QsX55vUs-SB4CZa4Nh4vvUF4EzW3D2r28C4o9Xd-VhBU13WVZJwLUTDdeSDqqu62O6T2p)

The solution has a bookshelf block as the perch but you could use any block you want.

![Perch for Better View 3](https://lh5.googleusercontent.com/rqSy3QXluq7XMtEZ4csaW4SOYn9DZfrW148c34A41eAiIdSfgYzm4BR2V6WGZGVJRzURnbuiHnC1c5Z6D39ZQMHhN7mJ6j7QrbraFeZzHFhtufyzUvaYwZX8l_X1b8HgNpqV6lAt)

#### Challenge 2 - Redecorate the Maze

Change what the maze walls are made of, the patches, and add a floor of a different block type. In total you would need to select 3 new block types to completely redecorate.

Block Types to Change:
1. Initial Maze or Block
2. Wall Patch (equip the agent with a different block for patching the holes it makes by accident)
3. New Floor

Answers will vary…

![Redecorated Maze](https://lh3.googleusercontent.com/5mW7ai5bE_aHhoIX6waES42mvcgm5D2MbQm7c8woCuUqgOW7EyrPIKeugBS5-2b0JacYmUOcUmbHj_-hDO34HI7rfM88vOI17_2hxKrB1E3rtEbWwIUk-rCZaKMDa36dOCM85LgG)

## Maze Pathfinding

- [minecraft.makecode.com /courses/csintro/ai/activity-2](https://minecraft.makecode.com/courses/csintro/ai/activity-2)

---

Now let’s teach the agent how to navigate a maze on its own. Rather than giving the agent a set series of directional commands to solve one particular maze, you are going to need to use conditional statements to teach the agent how to find its way through any maze, intelligently.

You first need a maze to start out with. In case you missed this, the code from the previous activity, [Maze Generation](https://minecraft.makecode.com/static/courses/csintro/ai/activity-1), builds a maze for you. The activity asks you to place a redstone at the end of the maze. This is how your code will know when the agent has finished the maze. The agent will detect this redstone under its feet to signal the end of the code.

![Stone maze with redstone at the end](https://lh6.googleusercontent.com/YjRAr7xryZ_ApUeGMqs76VcYM-ZEOwFF8aT2wU2t8ujmoj5m-ysUcY-WVu32J2v29gfEj0zwBDa7OQfU00nxW-b0lQT6qD64k7tmrZYQR_d-sZUKU6xsC1PCuzJrp2cWxlu2GfBK)

### The Algorithm

In any maze or labyrinth, you can always find your way out by following one wall consistently. You may not find the most direct way out, but you will always come out on the other side. In a Minecraft maze, this basically means always turn left whenever you can, and when you reach a dead end, turn around.

So, our simple maze-following algorithm looks like:
- As long as you aren't standing on redstone:
	- If there is no block to the left of you,
		- turn left and move forward.
	- Otherwise, if there is no block in front of you,
		- move forward.
	- Otherwise, if there is no block to the right of you,
		- turn right and move forward.
	- Otherwise,
		- turn around and move forward.
    

### Try to code it yourself

Try to code a way for the agent to get to the ending point on your own without following the activity steps. If the agent gets stuck, go ahead and use the steps to complete the program.

#### Make a new project
- Create a new MakeCode project called “Pathfinder”.
- Use this starter code from the [Introduction to the Agent](https://minecraft.makecode.com/courses/csintro/iteration/activity-1) activity.

This code allows you to easily position the agent.

~~~
player.onChat("tp", function () {
  agent.teleportToPlayer()
})

player.onChat("fd", function () {
  agent.move(FORWARD, 1)
})

player.onChat("lt", function () {
  agent.turn(TurnDirection.Left)
})

player.onChat("bk", function () {
  agent.move(BACK, 1)
})

player.onChat("rt", function () {
  agent.turn(TurnDirection.Right)
})
~~~

You can copy the preceding code by highlighting the code, pressing Ctrl+C to copy, and then pasting (Ctrl+V) the code into the JavaScript side in your code connection.

![Switch code to JavaScript view](https://lh3.googleusercontent.com/2MZVKWnL3wKQ0kBHcEkBNgO1TZ-DaYQIPYYh45UlMxu7e5KRkiZn8JAq40nG3rg5L_onqxul24WrKXVJK8WJoxdtCyEHADVIs398_sgREkJu1EFNnjzjwcLBuHm_B7m3xytWL6T-)

Let’s use the basic agent controls to move the agent to the starting point of the maze.

- Move your player to the start of the maze. Type the command “tp” into the chat window. Your agent should teleport over there. Then you will need to turn the agent left(“lt”) or right(“rt”) to get it facing inwards.

![Agent Sitting Just Inside the Door](https://lh5.googleusercontent.com/LINp6HZZ5DirQXWXFKjfP-UNG1Q2mhEDol9bqOmqbvIf6CogzqKVK1-uy-dephPegpOzU-uSWUTLyhwKDBKJ-_MmLIKGp3-Dky1ipascyXKTbQU2A0Zp1GG2HWpX_l0vVhLjoJ4d)

![Agent at Starting Location](https://lh3.googleusercontent.com/g_W8FuJGllu6p3GH2I2eUj1mqY4qLKtfjsxqdcyODMSYD2dt8iocFdUwTUbBs-t40WI_TGi7F2qoVAsSLR8ttcMYlOvJSN-l8_HI4Z1ZRzRfVk6k4pIlH92Py6swTMVsQFg_qA_5)

#### First Blocks
- Create an on chat command block and rename it to "mr" which stands for maze runner.
    
![](https://lh3.googleusercontent.com/unq_nTjQgk0gP5LbEpX998ZOTVl6XjxbONW4c40XLpnYR-AtIeF2Lodo0n7t1X5F5e1MfKvJYyPoOowe5uo040lFNgi7l7FJ_TISuuLwpBTxOz3ZQEUcZjpV5Lan_nrHGL6ZIVfY)

You’ll put the whole algorithm in a while loop, which will tell your agent to continue searching for the end of the maze as long as it isn’t standing on redstone.

- From LOOPS, drag a while loop into on chat command "mr".
- From LOGIC, put a not block into the while loop replacing the true.
- From AGENT, drag an agent detect into the not.
- In the agent detect block, use the drop-down menu to select redstone as the type of block to detect.
- In the agent detect block, use the drop-down menu to select down as the direction.
    
![](https://lh3.googleusercontent.com/hnoyb8Gdb7-Sx1wk6kJHhHfKbThaENOE6BFpqxOH7qVQkU_3tNt84VrCoYoccwRhaqP1YVdOjYPM2Zu70oS0XdXGfKOBOjg1C78J7CtMjQA2gdsYx71yxdnEZJjp2ak9C19nG0IS)

This essentially means that while the agent doesn’t detect redstone beneath it, your code will continue running.

#### Check for a path to the left

Next, we’ll check to see if there is a path open to the left and if so, turn left and move forward.

- From LOGIC, drag an if then else block into the while loop.
- Again from LOGIC, drag a not block into the if then conditional slot replacing the true block.
- From AGENT, drag an agent detect into the not block.
- In the agent detect block, use the drop-down menu to select left as the direction to look.
    
![](https://lh3.googleusercontent.com/Hx3u6c6zD44PdsaHiVxm--wQTwjmtGeM6zT9e40WgDTfP9WTxwl7zgrbfAdVqprHzNCVdIEX2EvzIGTmCGkKcTG8AnH3M62NcRCSJZ9sCVWVjCJys_KDXB6WU8I2izGgcSOzOrAm)

#### Turn and move forward

If the Agent doesn’t detect a block to its left, then we want the Agent to turn left and move forward.

- From AGENT, drag an agent turn, and an agent move block into the first branch of your if then.

![](https://lh4.googleusercontent.com/AQQ6P5gvi0vivsn-zlWlzdm1ZHyV6n4bje-eFyMJy57QUDi61K4yoV7moT_FjaP8vXt_qUflMCkZqRaXbmZTmC-puPdLQ2LC1han26IIVIP4PPUN7UyLJEQNq6FGBdx5S7NkvqLG)

#### Check for a path forward or to the right

Now we need to add 2 more conditions to check forward and to the right of the Agent.

- Click the Plus (+) sign at the bottom of the If then else block twice, to add 2 more Else if clauses.    

![](https://lh3.googleusercontent.com/mM8j7sbCM0LDkOoWjRTkuWsyUuNBZj15MaUtwYvTRv6laJKQO1EYi_Gw70uRBuy9WTo9-_I-ZjCYjNJrbujfH_Yk7TSsIH_xAMYH2jhLorFZLY5P0OKiJauLRkbXNvUMIRbUdQmU)  

#### Duplicate Conditions for the Other Branches of Your If
- Right-click on the not block in the first If then conditional slot, and select Duplicate – do this twice to create two more not agent detect conditions.
- Drop these duplicated conditions into the two additional else if slots.
- In the second branch of the else if, use the drop-down menu to select forward as the direction to check. Thus, we are checking left and then forward.
- In the third branch of the else if, use the drop-down menu to select right as the direction to check. Thus, we are checking left, forward, and then right.    

![](https://lh3.googleusercontent.com/hgydCgnfTkzhbe72pPH5Z-GvxG6UAwaJoNfvBYkCZssqU3_aUw70oTIHJG144G3p2yAkxwyBi199w7YOMGVGnyjrDe3HgkPNALFJGxU6zXwkmSx2tBPpcb-IQMHzG2k0UNWz2JUr)

  

#### Move ahead forward

If the agent doesn’t detect a block in front of it, then it should simply move forward.

- From AGENT, drag an agent move block into the second branch of the else if clause.    

#### Move along to the right

If the agent doesn’t detect a block to its right, then the agent should turn right and move forward.

- From AGENT, drag an agent turn, and an agent move block into the third branch of the else if clause.   
- n the agent turn block, use the drop-down menu to select right as the direction to turn.    

You may also want to just duplicate these blocks. That is perfectly fine as well!

![](https://lh3.googleusercontent.com/bEtSZg5ZS0c_1WgybFT8vdPd3-4U2X5ftaDHaCHKnGoRhARhM3JD7tZ15etnJq8gwFQizBn5CeSacutIgotnaDSnWq9eG1l-wAcKVrXHiwvXAeyNVs57lQ9ooTlRxrz-n7JrqJNg)

#### Turn around and go backward

Finally, if the agent is at a dead-end (none of the three directions are open), you want the agent to turn around and head back in the opposite direction.

- From AGENT, drag the following 3 blocks into the last else clause: 2 agent turn blocks, and an agent move block.    

![](https://lh5.googleusercontent.com/wWSFyW8fxD9aB65LOEABaTxGKxqanJ0MqY4snaBUuQFIbrwp7Xbs48amMPtgteACEO6wVXO6wVYtuU6eg1EFCnpGidwp2ivbdcjoF-5-lJlefDUM3Gh1-3_WJWS5fL919p6LUP5U)

#### Found the redstone!
- If the agent detects Redstone, it will know it has reached the finish. You can have the agent do a happy dance at the end of the maze! Feel free to reuse the code from the [Dance Dance Agent](https://minecraft.makecode.com/courses/csintro/iteration/activity-2) activity in [Lesson 5: Iteration](https://minecraft.makecode.com/courses/csintro/iteration).
    
~~~
player.onChat("dance", function () {
 for (let i = 0; i < 4; i++) {
   agent.move(LEFT, 1) 
   agent.attack(FORWARD)
   agent.move(RIGHT, 1)
   agent.move(RIGHT, 1)
   agent.move(RIGHT, 1)
   agent.turn(TurnDirection.Left)
   agent.move(LEFT, 1)
 }
})
~~~ 

- To run the code for on chat command "dance", place a run chat command "" block from PLAYER underneath and outside the while loop. It should read run chat command "dance" when you are finished.    

Using run chat command "dance" is like making a function call. You could use a function here instead if you wanted to.

#### Complete program

Shared Program: [https://makecode.com/_M8HXrKRLfhzM](https://makecode.com/_M8HXrKRLfhzM)

### Challenges

#### Challenge 1 - Fool the AI

How can you break this code or activity? Find a way to break this and describe why it confuses the agent or why it is not working.

#### Challenge 2 - Agent Feedback

Can you have the agent notify the player after the decisions it makes? The messages could say things like “Oh! Better turn left, I hit a wall!” There are several ways to do this.

![Agent Gives Feedback on Progress](https://lh4.googleusercontent.com/-_f4l7qtgy94gzJ-WeW-FNTU8K3CQLn0VmMhU26LNKJgt9f0tZfKNDN6ZIsACgLiqxp9ZRHqQ28deMbP1b6bLvdU4llvNWb9NykenS0LHppBxVLL60OaM7WpjZkAE0Fttd_UV6i5)

Can you find a way for the agent to mark the trail it takes. This might help others find there way through should they stumble upon the maze. The solution has the agent tilling dirt to show the way but perhaps you can think of other ways to mark the path.

![Breadcrumbs](https://lh4.googleusercontent.com/9q6KOeSVqQjQgDT-47yS3F1qdVTA-kdh051KOwfUHc9D-82VolBpX-5E263JM08XjuRDr6JuVowve_hewAu7DVvB1ZwE-MvCbEwRYiVadkXQVoWi9XGgmO_IeW0jTaEkSQji49eD)

![Breadcrumbs from Above](https://lh4.googleusercontent.com/N9KWT2RYkoJDyTZ1BJFuNKbJpxZuci4ALgbAzofRVnq5MTVAHRpHIOQOcOOK7w4DcagoufGV7ZVVL12vFRtAjXUi5P_KkQzryalDnCYTmpPYANRaoYEztDG68dMP8G61RjiCpFFh)

## Education Edition Setup for MakeCode

[minecraft.makecode.com /setup/minecraft-education-edition](https://minecraft.makecode.com/setup/minecraft-education-edition)

---

### Setting up Minecraft for MakeCode

Here’s how to get setup and connected to MakeCode for the first time…

#### Setup Minecraft
##### 1. Start

Start Minecraft and sign in if you’re using Minecraft: Education Edition.

##### 2. Create a world

Press the Play button. Push the Create New button in the Worlds dialog. The Create… window will have some default templates you could choose from but make your own world with the Create New World button.

##### 3. Turn on cheats

You’ll see some settings for your new world. Leave everything as you see it except for Cheats. You need to turn Activate Cheats to the ON position to enable all of the coding features for MakeCode.

##### 4. The world begins

Press Create and you can start playing in your new world.

##### 5. Start In-Game coding

Start in-game coding by typing “c“. The Code Builder window will show up in the game with a list of coding apps to choose from. Select Microsoft MakeCode.

![Choose MakeCode](https://lh3.googleusercontent.com/nHAnlVX5yR3077v1LYfkjwl0fPRBY30vK_ztJ358E5mFMfUkyR0nYsFBZViACRfucin1MZ7CXn85sYDytSmd6vwJy-t1W7woI8-S7NkbsOJ4lfFeRDGyygRl1nV6w5xq2pKtv_4p)

The MakeCode home screen will appear in the Code Builder window. Select “New Project” in the “My Projects” gallery to start a fresh project. If you want to try a tutorial or another example instead, pick one of those from the galleries.

![Select New Project or tutorial](https://lh5.googleusercontent.com/IhjWoqWrUjhSuyFDd5yRiLibjf6VNndOQG9bBw2eW3IrNUGmNiIed8cwuooiH2n3M0Crgy99csWu4FqmG4qESTqLKhJaREFQWIB5pCiq88RR-eZASlZDv_Egp_yaNKaf01el-PHh)

### Gameplay with your code

To run your code in Minecraft: Education Edition, go back to the game after working with your coding project. Press Resume Game. Depending on what your code is meant to do, your code might run as a chat command or maybe start when some condition in the game changes. Try one of the [tutorials](https://minecraft.makecode.com/tutorials) and follow the steps.

Minecraft has keyboard controls that help you move around and do tasks. Here’s a helpful key card that shows what they are:

![](https://lh5.googleusercontent.com/XV88XDem-J2RcV6J8z859uGSV_GY72nxgPy-zgTQumjVfjxrw24HUA5x0VXFnZ7AijiXgpKuJTWUfDusOG9iglPZeDaAcjWapEQIGLNfnZ38fOSTGWCFZFggq-NV50_cryLK0Wpy)

## How do I import a design into Minecraft?

- [https://www.instructables.com/How-to-Upload-3d-objects-From-the-Tinkercad-to-the/](https://www.instructables.com/How-to-Upload-3d-objects-From-the-Tinkercad-to-the/) 

---

You can view and edit your Tinkercad design in the "Blocks" editor and configure the block size and material before exporting it for Minecraft.

- In the editor, click the "Blocks" editor (pick axe icon).

![](https://lh3.googleusercontent.com/zjdy_HAnPyC7izJXIlgVcakJi41yQV4HlDJsV3Oo6iOtIW3r6TUvXsf1OQXhxZdZLiPSk-J75Qkv-VLqlT96zx3zrhA8YxgOwGpF64xVfS0fG47grhPHQ_Nl-XeTKDGHpE-zs3Fw)​

- You can change the materials for each object as you would like them to be in Minecraft. Just click the material to change it.

![](https://lh4.googleusercontent.com/Xf8ZqdZONG3RcvFNC_OE4XbFaxJdlfjF6Gd6BwV7Y1SERNZLjxX2BPT2EfbhLUC_mgUTvkWkkQQ2pq7haLViYyYFWSoTRtAWrqHXp7wPJaqRYhgMFIARVsuXPHztQyuwLiF6fYWH)

- Click "Export" to export your "blocked" design to a SCHEMATIC file (.schematic).

- Then, you can import the SCHEMATIC file into MCEdit (place it in your schematics folder) to place in your Minecraft worlds.

___

Actually, I did figure it out.
1. You can make worlds with MCedit.
2. then use the Anvil to LevelDB converter
3. compress the files into a zip folder. When you compress, compress the files, and not the folder, as you don't want an addition subdirectory
4. change the .zip to .mcworld, and then it will upload into Education edition
    

## How to Upload 3d-objects From the Tinkercad to the Minecraft World (Minecraft Education Edition)

- [zvereva.g.a](https://www.instructables.com/member/zvereva.g.a/) in [Teachers](https://www.instructables.com/teachers/)[3D Design](https://www.instructables.com/teachers/projects/?subjects=3d-design)16911

### Introduction

![How to Upload 3d-objects From the Tinkercad to the Minecraft World (Minecraft Education Edition)](https://lh6.googleusercontent.com/VehTh0G-s6iN4RQttO0d3u-CxN2s40c5ir5n91Vwoad8tK08Qu3WNzaPjovTGK1TQgtgHqvm1yj0SUW4ZsYEh8V88agPb8KZErwu82WlFfkkJoHySwMmCTeGpvfoYs6HDN8MH9ya)

Downloads:
1. 3d -objects from [https://www.tinkercad.com/](https://www.tinkercad.com/) in the format .schematic
2. Minecraft:Education Edition: [https://education.minecraft.net/get-started/downl...](https://education.minecraft.net/get-started/download)
3. MCedit: [https://www.mcedit-unified.net/](https://www.mcedit-unified.net/)
4. Amulet: [https://github.com/Amulet-Team/Amulet-Map-Editor/...](https://github.com/Amulet-Team/Amulet-Map-Editor/releases/tag/0.7.2.8)
    
### Step 1: Step 1

![Step 1](https://lh4.googleusercontent.com/1n_wECtH5MtkAMhqdeCCbkNJIY28l18-qc8LZssa7kyAnh3KAGafUkOLOyGFKNtyiRn9Sjk5nI6inwf0XfDC1b3nKJms8A8yRUx7uXh_rc0prUG_GnUE7uXsRTnCK5pGR2xngUfa)

Choose ”Blocks” presentation of the object, appropriate design size and export your object in the format .schematic.

### Step 2: Step 2

![Step 2](https://lh4.googleusercontent.com/k_SVs9usITi5TbR0u719IToM9ZWCIEYCLf_dTqi5S_rbDaS1H_jgRqkYosKy53Xin5315XZEgVHMP0khjsUr5BACn2yA0tT92IlpJ1S5_-X-LWJ9yrU7rx8r1sPJ5AhMXUbTwMPz)

Install and log in to Minecraft: Education Edition (M:EE) in accordance with direct instructions from the site. Create a new world, save or export it. We recommend using the following settings: creative mode, easy difficulty, flat type. Worlds automatically are saved by the following links C:\Users\AppData\Roaming\Minecraft Education Edition\games\com.mojang\minecraftWorlds.

### Step 3: Step 3

![Step 3](https://lh5.googleusercontent.com/OFT8PZOOek-xNl5GqKMThcQTfV0AVMdcmoJzB0YveRGhOUdFVxRdZ7fSsF61N1KjvqiGkZBRWae43Y9Gx27xfLA1XSk_2DVvPlKhpuOaqiWxP1D7QgLr7BhHb4Q95TAgmJyMfs5P)

Download MCedit in .zip and unpack it, launch the application. Click the button “create a new world” and use the recommended setting: creative game type, flatland generator. Import in this world 3d objects from Tinkercad using, for example, this guidance. [https://www.youtube.com/watch?v=Ur60XFRZvEU&ab_ch...](https://www.youtube.com/watch?v=Ur60XFRZvEU&ab_channel=ChrisAviles)

Save the mcedit world on your computer and quit from this application. NB! Before launch MCedit close M:EE.

### Step 4: Step 4

![Step 4](https://lh6.googleusercontent.com/M2303iQ8z2mgIX6JftL7cAJrOJQCbVb08XetpF8ySXlqJvjas30BhYQVO-Sr3IBopJhACd3aaybzsNtqCPBL58Y2RN8NLEcQUm18uiX36oamh99QlcxPQwHOnpfF-4pbe4d-lVj1)

Download Amulet in .zip and unpack it, launch the application. Select input World (Mcedit) and Output World (M:EE) in the tab “convert” and click “convert”. Changes should successfully convert to the M:EE world, which automatically is saved in the M:EE storage (see link in Step 2).

### Step 5: Step 5

Check that you have the world with the Tinkercad objects in the M:EE, host it and invite friends to join your world.
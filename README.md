# GDIM32 In Class Activities

## W8
### Activity 1:
Took notes about rendering pipeline and post-processing effects in notion

[My notion note](https://www.notion.so/Rendering-312fca0abb9d8027bdfaff3f39edec5d?source=copy_link)


## W7
### Activity 1:
While running through the demo, I reviewed the code for FSM and read the codes through thoroughly. Also, I found the duck NPC's auto-following function exactly the thing we need for our project, where the monster will be a NPC checking its distance with the player and run toward the player. This demo will be a great basis for our Monster movement script, and we will apply the similar usage of raycasting and gizmos for better visualization of our work. 

### Activity 2:
Attendence for Nameless group: Jingyi

### Activity 3:
![Final Breakdown](https://github.com/user-attachments/assets/8503d99e-8b1c-41da-8af3-8e570edcfa2e)

### Activity 4:
We shared a trello task table~
Current task assigned:
Jeremy: Start with the monster script, implement basic gameObjects
Averin: Looking up for 3D models, plannng the terrain

### Activity 5:
Import the texture and tree models for future use. Tried with implementing the tree prefabs but currently failing because the model looks like a bunch of weird 3D pillars. 


## W6
### Activity 1:
- For the demo about optimization, I found the Profiler function EXTREMELY COOL!! It gives me important insights about why the optimization in the large games I played often seem so hard and complicated. Sometimes the precisions about game details have to be sacrificed for the important mechanics to perform better, such as how in FPS games the textures of materials are simplified for players to have a smooth shooting experience. 
- The demo about gizmos is really fascinating. By the only time I've got used of gizmos to outline the camera perspective for me, I've never thought how gizmos could help programmer this much, in accurately tracking all these physics components of a game object just as shown in the example. It would definitely get a lot of use in my future projects and career. 
- The demo about breakpoint is helpful for debugging. Haven't have chance to try it but it's certainly useful in the case of game designing, since programmer has to deal with multiple scripts at a time. I would start getting use to it when I find that simply "proof-reading" the scripts might not be enough for debugging XDD.

### Activity 2:
Attendence for Nameless group: Jingyi, Jamin

- We deleted the "Inheritance and Polymorthism" section because it's not really applicable to our game and we already have other three decent architecture systems. We also solidify our plan by deciding the environment to be forest, the NPC to be a friendly villager, and searching for the 3D model of the antagonist. 


## W5
### Activity 1:
In this activity, the thing I've observed is that most of the compile error happens because the child classes fails to implement the required methods from the parent (interface or abstract), didn't use the intended modifier, or that the override was forgot. For me, I actually found this type of inheritance useful, in the purpose of establishing the "defaults methods" that must be correctly implemented by the child classes and that "shouldn't be forgot". These compile errors would act as a good reminder when I forgot to implement some key features for these classes. Although the structure seems complicated at first, it's very logical after decomposing and looking detailedly into its working logic. Inheritance would definitely be useful as the project evolves in size, and I would want to implement these design patterns to make my code more professional. 

### Activity 2:
- Model -> the scriptable objects represent the model part because they are data structures that handle the most fundamental logic of the game
- View -> inventory UI handles the display of inventory to the screen, as well as the dialogue class
- Controller -> player class controls the central mechanism for the game to work

### Activity 3:
#### Scenario 2: team shooter
In team shooting game, we think the model represents the data and stats for the tools, projectiles, and weapons, and they are encapsulated by scriptable objects. The view is displayed as the UI, players on-screen movement, map, and the scoreboard. As for the controller, it controls and manipulates the actions and logics of them, and the conditioning (like killed or picked(grab something to the inventory). Most of the controller and manager (like gamecontroller, UImanager, audiomanager) will exist as singleton for easier reference. 

A major component to do with inheritance is the type of weapons. The parent class could be Guns, Projectile, Knife, and there would be specific weapons that inherited from these parent classes. Polymorphism is useful for coding the required features for the weapons, such as the public method AmountofDamage, inherited variables like ammo. 

### Activity 4:
Attendence for Nameless group: Jamin, Jingyi

[Proposal First Draft](https://docs.google.com/document/d/1243b-56SntC6QbFu_Eii6tyaacd2RoO3u3ZMJNCXjdw/edit?usp=sharing) 

## W4
### Activity 1:
Partner name: Jingyi Cheng

Add multiple Locator objects to the Scene. What happens to the Locator objects when you run the game, and why?
- Only one among all the scripts will remain, the other locator is destroyed (only the scripts are destroyed not the gameObject it attached to).


### Activity 2:
![MG4 Breakdown](https://github.com/user-attachments/assets/22a77f76-cb9a-4bac-a0cd-2dd919675ff5)

### Activity 3:
![in-class commit history](https://github.com/JeremyC140/mg4/commits/main/)

Spent most of the time setting up the sprites, rendering their images, and building their colliders. Finished lower, mid, upper pipes logic (basically the entire pipe prefabs' appearance) and the player sprite :))

## W3
### Activity 0-2:
Partner name: Jingyi Cheng


### Activity 3: MG3 Breakdown
![IMG_2934](https://github.com/user-attachments/assets/746d7526-dd71-4e2f-846c-739bdf2079db)


## W2
### Activity 1: MG2 Breakdown
![IMG_2841](https://github.com/user-attachments/assets/acfa7e29-acb1-4381-b2d9-4b4c00131259)


### Activity 2: MG2 Progress
[Commits Made](https://github.com/UCI-GDIM32-W25/mg2-JeremyC140/commits/main/)
I finished the assets setup, the jumping of penguin (and isGrounded check), the UI with TMP_text (but not yet the update part), collision check in the penguin script, and attempt on the coin moving script as well as the game controller. 

TO-DO:
- Fix coins not moving
- Assign enough variables to update the text 


## W1
### Activity 1:
- My advice: don't miss every of the little details in the rubric
- Table advice: read the rubric line by line, ask questions when stuck, don't procrastinate


### Activity 2:
- Q1: x = 10

- Q2: x = 2

- Q3: The Update function calls another private method called PrintMessage (), which sends a log of "hello world" to the console, for every frame that unity runs. 

- Q4: public class Example: Monobehaviour

- Q5: The Start function calls another private method called PrintMessage () embedding 10 as the parameter, which the method then sends a log of "x = 10" to the console, for only once when the game starts running. 

- Q6: the 10 in the parenthesis is the parameter that was sent to the method PrintMessage(), and as the method's argument x receives 10, "x = 10" is printed.

- Q7: The Transform is not defined and the computer wouldn't know which object it's supposed to translate.  

- Q8: Thus, Transform is supposed to be altered to _playerTransform in order to correctly assign the object for translate.


### Activity 3:
[MG1 breakdown](https://docs.google.com/document/d/1Ze4Iwr71L5shh5hsj0SjaYT7WLsAfV0lCdb13onncaA/edit?usp=sharing)


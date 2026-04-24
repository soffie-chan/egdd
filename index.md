# Linkin' Chickin

## Elevator Pitch

An outcast blue baby chick goes on an adventure to find his mother hen, Mama. Using linked list logic to connect each platform, it's up to you to traverse, insert, and delete platforms to help Baby Blue!


## Influences (Brief)

- *Duck Life*:
  - *Game series about raising a duck to be a champion in a sport.*
  - Sprite animations

## Core Gameplay Mechanics (Brief)

- Jump to platforms by solving platform-connection problems (related to linked lists)
- Delete platforms with threats to eliminate them.
- Incorrect platform connections  lead to injury, enough of which can lead to death (replaying the level)
- Correctly connect platforms to ensure that the chick can jump to them AND reach his end goal.
- Traverse the platforms using buttons and delete dangerous spiky platforms to advance.
- Fight boss battles to test your knowledge
- View how your moves correspond to real code in an on-screen box.

# Learning Aspects

## Learning Domains

C++ and Linked Lists

## Target Audiences

* Intermediate-level programmers with understanding of C++, who are starting to learn data structures and linked lists.

## Target Contexts

* This would be assigned as a supplementary learning material for a student enrolled in C++ or Data Structures courses.

## Learning Objectives

- By the end of the lesson, players will be able to, when given a linked list, sequence pointer assignments for insertion, deletion, and traversal.
- By the end of the lesson, players will be able to perform necessary actions to remove, add, and travel through doubly linked lists.
- By the end of the lesson, players will be able to, when given a linked list, identify how incorrect assignments cause loss of references or broken lists.
After completing the game, the player will demonstrate:
- The ability to traverse, delete nodes, and insert nodes in linked lists.
- The ability to visualize the loss of reference nodes or creation of a broken list when traversing linked lists.

## Prerequisite Knowledge

- Prior to the game, the player needs the ability to code in C++ and demonstrate basic coding capabilities, including datatypes, varibles, loops, and other basic coding knowledge.
- Prior to the game, the player needs to demonstrate knowledge of the structure of a node, including the .next and .prev fields.

## Assessment Measures
A short pre-test and matching post-test (where the data numbers are randomized each time) should be designed to assess student learning.
- Given data, create nodes including the data and arranging them in the provided order using .next fields.
- Given the nodes and a sequence of .next and .prev, traverse the list and find the data that it points to.
- Choose one data point and delete it from the linked list. Choose a new point and insert it into the linked list.

The following is an example of the assessment -
A Node class is defined as the following -
class Node {
  data: int;
  next : NULL;
  prev: NULL
}
The following list - H-[12, 7, 25, 3, 18, 5] -T - contains nodes. Each number shown is their data, stored in a pointer called "node<data>". For example, 12 is the data of node12, where node12 is a pointer.

- Given the nodes with data of 7, 5, 3, 18, 25, 12 , Fill in each node's .prev and .next field to arrange them in the order presented in the list above.
`
node12->next = node7;
node7->next = node25;
node25->next = node3;
node3->next = node18;
node18->next = node5;
`
`
node7->prev = node12;
node25->prev = node7;
node3->prev = node25;
node18->prev = node3;
node5->prev = node18;
`


- From the now ordered linked list, insert the node with data of 14 between the nodes with data 25 and 3. Assume the data of 14 is stored in a node 'node' with .prev = NULL and .next = NULL.
`
node14->next = node3;
node14->prev = node25;
node25->next = node14;
node3->prev = node14;
`

- Delete the node with data of 5.
`
node18->next = NULL;
delete(node5);
`

- Traverse the list and print each node in the order provided in (1).
`
Node* temp=node12;
while (temp!=NULL){
  cout<< temp->data<<" ";
  temp = temp->next;
}
`


# What sets this project apart?

- This project explains the traversal of a linked list to a player - a concept that is hard to visualize with static imagery and words alone.
- This project also allows the player to understand the loss of reference points or result in a broken list if incorrect platforms are connected to previous ones, which is much harder to do in code alone.
- This game also allows the player to use attacks that test how the players set up their nodes, ensuring that everything is connected to prevent punishment.
- This game allows the player to have to complete the ordering of nodes or platforms in a prompt manner in boss fights, testing the grasp of knowledge and reaction time.

# Player Interaction Patterns and Modes

## Player Interaction Pattern
Linkin' Chickin is a single-player game. Only one player is involved at once. They will primarily use the mouse of a computer to make connections between platforms, progress the player, and click through options and cutscenes.

## Player Modes

- *Player Menu*: Consisting of a Quit, Play, and Options button, the player can click the buttons to close the game, play the game, and change the settings within the game respectively.
- *Cutscenes*: There is no active gameplay or learning in these scenes - they are mostly pictures with a caption of dialogue under them to progress the story.
- *Gameplay*: Single-player gameplay where you advance through the level based on performance according to the rules. There are three total stages with 3-4 levels in them each until the end.

# Gameplay Objectives

- *Connect the platforms*:
    - Use proper code to connect the "previous" and "next" field of each platform on the screen.
    - *Learn how to insert and delete nodes in a linked list and how .next and .prev work based on an address.*
- *Jump to different platforms to progress after connecting them*:
    - Use proper node connection to go to different platforms to go to the end of the level from the start.
    - *Learn how to traverse through a linked list.*
- *Defeat enemies*:
    - Delete the nodes that enemies are standing on and find your way through mazes of platforms.
    - *Provide a sense of achievement on wins, but punish mistakes when hurt*
- *Advance through levels*:
    - Successfully make it to the end of the level.
    - *Complete varying difficulty levels of the concept at hand.*
- *Advance through stages*:
    - Successfully complete 3-4 levels and defeat a boss battle related to the same topic.
    - *Complete learning a concept related to linked lists.*

# Procedures/Actions
- The player can use the arrow keys to move Baby Blue across different platforms, which works only when platforms are connected.
- The player can type linked-list-related commands into a text box to connect various nodes (platforms)
- The player can delete or insert new platforms depending on their availability and the stage.

# Rules

- The player has a text box at the bottom of the screen. They use this box to enter commands that connect various platforms across the level. Helpful tips will be given in the first level of each stage.
- They player uses arrow keys to move the main character around the level and uses them to jump from platform to platform.
- The player must use .next or prev to connect platforms before jumping, showcasing how linked lists function without proper connections.
- Players must reach the end objective (listed at the upper left of the screen) to complete the level. It can range from collecting items to simply reaching a platform.


# Objects/Entities

- Main Character and their features - including their movement and their healthbar.
- Bosses.
- On-screen text box for commands
- Platforms.
- Trina Saurus tips and tricks during the stage.
- Announcements. (You win, You lose, Stage Complete, etc.)
- Buttons (Main screen, settings, quit, restart, etc.)

## Core Gameplay Mechanics (Detailed)

- Jump to platforms by solving platform-connection problems (related to linked lists). Traverse a linked list path and be able to choose which platform is next based on which nodes (platforms) are connected to the current node.
- Stealthily execute unaware opponents with action combos. Sneak up on opponents at different parts of the platforms if you perform the right node operations. Advancing to more difficult enemies leads you to a boss fight, which is similar in combat, but timed - you lose your turn if the timer runs out on your move. Use your knowledge of linked lists and their connections (links) to link platforms to avoid attacks. Answer questions in a limited amount of time, and finish the boss level to advance to the next topic.
- Incorrect platform connections and not-so-stealthy encounters lead to injury, enough of which can lead to death. As you connect platforms, choosing two in an incorrect order/sequence could cause damage to the health of your player. Additionally, failing to sneak up on opponents can lead to similar injury and loss of health. If player sustains enough damage, it will result in death, causing the player to have to restart the level.
- Traverse the platforms using buttons and delete dangerous spiky platforms to advance. Cross platforms via Previous and Next nodes respectively. Delete dangerous, spiky platforms (ones that would not connect via links) in order to advance past them to more suitable and correctly sequential platforms.
- Players can view and type in a small box on the screen to understand the actual code behind their operations.

    
## Feedback
**Short Term Feedback**
**VISUAL**
- The player is rewarded with an "Enemy Slain" popup when they kill a regular enemy. They will have an enemy counter to help them see how many they killed. Lastly, once all enemies are killed, they will have a "All enemies slain. Move forward." text popup.
- In the start of the game, the tutorial will be led by a snake spirit that will be very encouraging, saying things like "Good work, you made it to the next platform!" and rewarding the player for their moves. Around the fourth stage, when he fades away, he will reassure the player that they know the most important things to progress forward.
- The stages will be white screens with the stage name and title written on it, so the player is fully aware of their progress.
- On making too many mistakes, the player will die, recieving a black screen that gives them some words of advice based on the reason why they died.

**AUDIO**
- The main character will make a chirping sound when they get hurt, signaling that the player made a mistake, paired with a decreasing healthbar.
- A victorious sound will play on level completion.
- The background music for each level features a soft song paired with natural environment noise.

**ANIMATION**
- Baby Blue jumps from one platform to another and can walk around on platforms.
- There will be one "empty area" that the player can run through - signaling a boss battle is incoming and that they are at the final stretch of the gameplay objective of that stage.

**Long Term Feedback**
- A level and stage counter will inform the player of their progression through the game.
- When you win a stage, you get a cutscene into the next stage. When you win the game, you get a more detailed cutscene where Baby Blue finds his Mama.
- If you make an incorrect connection, you will start at the beginning of the level. The player will recieve a blurb that appears on the top of the screen as to how the character got hurt.
- On completing levels, the player will recieve a congratulatory message.


# Story and Gameplay

## Presentation of Rules

- As a chicken, Baby Blue is bound to have a dinosaur ancestral spirit. This spirit guides Blue throughout the game at the first level of each stage.

## Presentation of Content

- Players will receive a short tutorial from a dinosaur spirit (see **Presentation of Rules**).
- Since the concept at hand is linked lists, each node is a platform, whose data can be plain, with an enemy, with spikes, or with items. This will be a visual detail that the player is expected to grasp. Each platform will have a small Japanese character representing an "address" to the next or previous platform. This will teach players on how linked lists are formatted.
- The player will have a text box on the bottom right that allows them to enter different node connections to connect platforms. Furthermore, players will have hints written on walls at times.


## Story (Brief)

Mama is a great mother hen who has taken care of many babies over years in the barn. She anxiously awaits her new chick's arrival... only to find out that he's blue! Baby Blue is often outcast by his coopmates and therefore closer to Mama, who teaches him strength. One day, Mama is taken away from the farm to be turned into chicken tenders. The coop accepts it as a part of life, but Baby Blue and his trustworthy ancestor's spirit, Trina Saurus, make it their mission to find Mama.

## Storyboarding
(Not here yet)

# Assets Needed

## Aesthetics

Linkin' Chickin is meant to have a very cozy, comfortable art style to give players a calming atmorsphere. The graphics are hand-drawn with paint brushes, making the environment feel like a painting.


## Graphical

- Characters List
  - *Baby Blue* - Main protagonist, controlled by player.
  - *Trina Saurus Rex* - Guide to assist player during first levels.
  - *Mama* - The mother hen that Baby Blue attempts to save.

- Textures:
  - *Characters* - Characters are in a painted, gouache, comic art style
  - *Cutscenes* - Non-animated scenes of cartoons in gouache
  - *Environment* - Varies based on stage. Stage 1 is in a barn, stage 2 is in a plains/forest area, and stage 3 is in the city.
  - SEE **STORYBOARDING** FOR VISUAL DETAILS!

- Environment Art/Textures:
  - Each stage has its own background as you approach your destination - from the within a barn, to a vast valley outside of it, to a city.
  - The platforms are designed based on their stage - for example, hay platforms in the barn stage.

## Audio

- Music List (Ambient sound)
  - *Main Screen/Death Screen*: [Bamboo Flute Music](https://youtu.be/kIQS15N5qYQ?si=xXjXFNbwLzA-9-rW)
  - *Boss Fights*: [Battle Music](https://youtu.be/E9kfzk0ei88?si=8dvjtMh9ynD3Q598)
  - *Mid-Level*: [Ambient Japanese Instrumental](https://www.youtube.com/watch?v=RWKnJn-gVxw&list=RDRWKnJn-gVxw&start_radio=1)
  
- Sound List (SFX)
  - *Attacks*: [Sword Slashes](https://www.youtube.com/watch?v=4bJI-e28kFg)
  - *New Stage*: [Sound Effect Music](https://www.youtube.com/watch?v=YOTDFFImDb0)
  - *Main Menu/Options Select* (Clicking Play/Options/Quit/Menu): [Slash](https://www.youtube.com/watch?v=aqXcGxcfUXQ)
  - *Jumping/Landing*: Short grunts and gasps (as heard in games like Temple Run). We intend to record these by ourselves!


# Metadata

* Template created by Austin Cory Bart <acbart@udel.edu>, Mark Sheriff, Alec Markarian, and Benjamin Stanley.
* Version 0.0.3

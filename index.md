# The Last Shinobi

## Elevator Pitch

A ninja in training receives a mysterious letter from a captured village, from his long-lost brother in his deathbed, who wishes to see his shinobi brother once more. However, the path to him is not easy - the land is overrun by enemies that are only reachable through connecting, deleting, and traversing nodes as you would with a linked list. Time is running out - if no one can fight for the last shinobi, he will do it himself.


## Influences (Brief)

- [*Shadow Fighter*](https://www.youtube.com/watch?v=CTHdMReN_9I&list=PLGtZwVE-T07sgNHY4O-rWxXGvv_iazHaA):
  - *Video game with Player vs PC action fighting (Mobile)*
  - *The combat animations, environment design, and character profile designs.*
- [*Ronin: Turn-Based Action Platformer*](https://www.youtube.com/watch?v=zLmbeogBfqU):
  - *Video game with Player vs PC turn-based fighting*
  - *Turn-based combat and action, level design with platforms, and overall "feel" of the game.*
- *Naruto*:
  - *TV Series (Anime) based on a young, rising ninja facing troubles.*
  - *Character design, special effects, main art style, and the concept of "fighting styles" (jutsus) used as power-ups.*

## Core Gameplay Mechanics (Brief)

- *Jump to platforms by solving platform-connection problems (related to linked lists)*
- *Stealthily execute unaware opponents with action combos*
- *Incorrect platform connections and not-so-stealthy encounters lead to injury, enough of which can lead to death (replaying the level)*
- *Correctly connect platforms to ensure that the shinobi can jump to them AND reach his end goal.*
- *Traverse the platforms using buttons and delete dangerous spiky platforms to advance.*
- *Fight boss battles to test your knowledge against the clock*

# Learning Aspects

## Learning Domains

*Briefly list any and all of the disciplines and learning domains for this subject.*

## Target Audiences

*Who are your learners?*

## Target Contexts

*Describe what kinds of formal and informal learning contexts this will be used in (e.g., courses, k-12 computer labs during free time).*

## Learning Objectives

*Remember, Learning Objectives are NOT simply topics. They are statements of observable behavior that a learner can do after the learning experience. You cannot observe someone "understanding" or "knowing" something.*

- *By the end of the lesson, players will be able to, when given a linked list, sequence pointer assignments for insertion and deletion.*
- *By the end of the lesson, players will be able to, when given a linked list, sequence pointer assignments for traversal.*
- *By the end of the lesson, players will be able to, when given a linked list, identify how incorrect assignments cause loss of references or broken lists.*

## Prerequisite Knowledge

*What do they need to know prior to trying this game?*

- *Prerequisite Learning Objective #1*
- *Prerequisite Learning Objective #2*

## Assessment Measures

*Clearly identify a set of viable assessment questions AND their grading logic. The questions should be specific examples of the kinds of questions that your game could conceivably improve student performance on. For the grading logic, it could be the correct answer, a rubric for evaluating the answer, or exact logic for deriving answers.*



# What sets this project apart?

*Give some reasons why this game is not like every other game out there. Whether the learning objective is unique, the gameplay mechanics are new, or what. You should persuade the reader that your game is novel and worthy of development. Consider arguments that would be persuasive to a Venture Capitalist, Teacher, or Researcher. These might be focused on learning needs, too.*

- *Reason #1*
- *Reason #2*
- *Reason #3*
- *Reason #4*
- *etc.*

# Player Interaction Patterns and Modes

## Player Interaction Pattern

*Describe how people play your game, how many players are involved at once, how they interact with the system works, etc.*

## Player Modes

*Your game has one or more player modes. Describe each discrete mode, considering things like menus too. Generally describe the transitions between modes too.*

- *Player mode #1*: *Description*
- *Player mode #2*: *Description*
- *etc.*

# Gameplay Objectives

- *Primary Objective #1*:
    - Description: *Description*
    - Alignment: *Describe how this aligns with one or more learning objectives*
- *Primary Objective #2*:
    - Description: *Description*
    - Alignment: *Describe how this aligns with one or more learning objectives*
- *etc.*

# Procedures/Actions

*Describe the control scheme and what actions a user can take in the game.*

# Rules

*What resources are available to the player that they make use of?  How does this affect gameplay? How are these resources finite?*

# Objects/Entities

*What other things are in the world that you need to design? These may or may not directly translate to actual objects and classes.*

## Core Gameplay Mechanics (Detailed)

- *Jump to platforms by solving platform-connection problems (related to linked lists) - traverse a linked list and be able to choose which platform is next based on which nodes are connected to the current one.*
- *Stealthily execute unaware opponents with action combos. Sneak up on opponents at different parts of the platforms. Be able to perform action combos to take out these opponents. Fight boss battles to test your knowledge against the clock. Use your knowledge of linked lists and their connections (links) to one another. Answer questions in a limited amount of time, and compete against bosses.*
- *Incorrect platform connections and not-so-stealthy encounters lead to injury, enough of which can lead to death. As you connect platforms, choosing two in an incorrect order/sequence could cause damage to the health of your player. Additions, failing to sneak up on opponents can lead to similar injury and loss of health. If player sustains enough damage, it will result in death, causing the player to have to restart the level.*
- *Traverse the platforms using buttons and delete dangerous spiky platforms to advance. Cross platforms via WASD keys to go up, left, down, and right, respectively. Delete dangerous, spiky platforms (ones that would not connect via links) in order to advance past them to more suitable and correctly sequential platforms.*

    
## Feedback

*Explicitly describe what visual/audio/animation indicators there are that give players feedback on their progress towards their gameplay objectives (and ideally the learning objectives).*

*Describe what longer-term feedback you detect and give that guides the player in their learning and lets them know how they are doing in regards to the learning objectives.*

# Story and Gameplay

## Presentation of Rules

- As a practitioner of Hebijutsu, The Last Shinobi is connected to his environment, specifically the nature of snakes. A snake spirit will provide helpful dialogue to assist the shinobi in his trials, especially in the beginning, that will disappear with time. This spirit is later revealed to be the Shinobi's brother's fighting spirit.
- When injured enough times to die, the player will be faced with a black death screen and the white silhouette of the last shinobi in his death animation. Depending on how the player failed (lost connection to a platform, died to a platform that should have been deleted, etc.), they will receive a helpful note surrounding the topic of the stage.
[PICTURE HERE]

## Presentation of Content

- Players will receive a short tutorial from a snake spirit (see **Presentation of Rules**).
- Since the concept at hand is linked lists, each node is a platform, whose data can be plain, with an enemy, with spikes, or with power-ups. This will be a visual detail that the player is expected to grasp. Each platform will have a small Japanese character representing an address, which will be used to complicate the game later on. This will teach players on how linked lists are formatted.
- The player will have buttons on-screen to move to the next platform ('.next'), to go back to a platform ('.prev'), and to commence an attack. If the player goes to the platform in the right sequence, they will be able to do a critical surprise attack, killing the enemy in few hits. However, if done incorrectly (for example, if they delete a platform they are standing on and end up falling onto the platform below them that contains an enemy), they will be punished by being attacked and recieving damage. Enough damage will kill the player and force them to start from the beginning of the level. This teaches core elements of linked lists, such as traversal, deletion, and insertion.
- Boss levels will have the same features, but the player is timed. The level will be set in a specific way that pose some concepts as puzzles (for example, the player will be expected to created a doubly linked list to travel backwards to dodge an incoming attack). Note that the player is not allowed to stay on the same platform at any point in the game.

## Story (Brief)

The Last Shinobi is one of the last disciples of Hebijutsu. The ninja, once given up to his training as a young boy, lost contact with his family, including the brother he once looked up to - a trained swordsman who returned from war with a strange illness. With all his hopes gone up in the flames along with his village, the shinobi recieves a secret letter from his brother, who now hides in a nearby village captured by their clan's greatest enemies. The news is devastating - his brother lies on his deathbed, with the last hope of seeing his brother once more before he rests. Determined, the shinobi prepares his sharpest sword for the greatest battle of his life - not just him against the strongest clan in ancient East Japon, but the force that kept him from his soulmate for far too long.

## Storyboarding

[PICTURES HERE]

# Assets Needed

## Aethestics

*Give a sense of the aesthetics of your game, the spirit and atmosphere. Use descriptive, evocative words that can help the reader understand the emotional response of your game.*

## Graphical

- Characters List
  - *Characters 1*
  - *Characters 2*
  - *...*
- Textures:
  - *Texture 1*
  - *Texture 2*
  - *...*
- Environment Art/Textures:
  - *Environment Texture 1*
  - *Environment Texture 2*
  - *...*


## Audio


*Game region/phase/time are ways of designating a particularly important place in the game.*

- Music List (Ambient sound)
  - *Game region/phase/time*: *Example 1*, *Example 2*
  - *Game region/phase/time*: *Example 3*, *Example 4*
  
*Game Interactions are things that trigger SFX, like character movement, hitting a spiky enemy, collecting a coin.*

- Sound List (SFX)
  - *Game Interaction*: *Example 1*, *Example 2*
  - *Game Interaction*: *Example 3*, *Example 4*


# Metadata

* Template created by Austin Cory Bart <acbart@udel.edu>, Mark Sheriff, Alec Markarian, and Benjamin Stanley.
* Version 0.0.3

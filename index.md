# The Last Shinobi

## Elevator Pitch

A ninja in training receives a mysterious letter from a captured village, from his long-lost brother in his deathbed, who wishes to see his shinobi brother once more. However, the path to him is not easy - the land is overrun by enemies that are only reachable through connecting, deleting, and traversing nodes as you would with a linked list. Time is running out - if no one can fight for the last shinobi, he will do it himself.


## Influences (Brief)

- [*Shadow Fighter*](https://www.youtube.com/watch?v=CTHdMReN_9I&list=PLGtZwVE-T07sgNHY4O-rWxXGvv_iazHaA):
  - *Video game with Player vs PC action fighting (Mobile)*
  - The combat animations, environment design, and character profile designs.
- [*Ronin: Turn-Based Action Platformer*](https://www.youtube.com/watch?v=zLmbeogBfqU):
  - *Video game with Player vs PC turn-based fighting*
  - Turn-based combat and action, level design with platforms, and overall "feel" of the game.
- *Naruto*:
  - *TV Series (Anime) based on a young, rising ninja facing troubles.*
  - Character design, special effects, main art style, and the concept of "fighting styles" (jutsus) used as power-ups.

## Core Gameplay Mechanics (Brief)

- Jump to platforms by solving platform-connection problems (related to linked lists)
- Stealthily execute unaware opponents with action combos
- Incorrect platform connections and not-so-stealthy encounters lead to injury, enough of which can lead to death (replaying the level)
- Correctly connect platforms to ensure that the shinobi can jump to them AND reach his end goal.
- Traverse the platforms using buttons and delete dangerous spiky platforms to advance.
- Fight boss battles to test your knowledge against the clock

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
- The player can click the "Next" button to move to the platform that is linked to the current platform's "next" field.
- The player can click the "Previous" button to move to the platform that is linked to the current platform's "previous" field.
- The player can click "Attack" to use their turn to fight an enemy. Combat is a Quick Time Event that will do damage to the opponent based on how well it was executed.

# Rules

- The player has a "Next", "Previous", "Attack" button at the bottom of the screen. They can use these to move the main character himself.
- Clicking on a platform will allow the player to "edit" its characteristics. Each platform will have a Japanese character on its left (previous address) and right (next address). The player has to click the proper character (left or right) and then click the correct  character on the next platform to connect the two. There will be multiple platforms, so connecting them will advance in difficulty.
- The player can only interact with the middle section of the screen. The screen has a left section (where the main character is standing), a middle section (whose platforms have editable properties) and the right section (whose platforms cannot be edited, but can be jumped to - this becomes the middle section after the previous platform is solved correctly).
- Eventually, the previously mentioned "middle section" will get much larger, allowing players to move around more, but make even more mistakes.
- The player is not allowed to stay on the same platform at any point in the game, forcing them to move forward or backward depending upon the level design to prevent players from not making a decision.
- The player only gets the assistance of a "snake spirit" on the first stage, which is an introduction to the game. After that, they only get hints to a better performance on the death screen.
- The player will be given a QTE (Quick Time Event) to attack an opponent. Its difficulty will vary based on how "clean" their platform connection is. Players are required to kill all enemies before proceding, and cannot do so by deleting their platform.
- Players will learn through these steps to traverse a linked list. Furthermore, difficulty will be enhanced with an increasing number of nodes (platforms), and concepts including:
  - node deletion (removing a harmful platform)
  - doubly linked lists (in the first stage, the player can only move in one direction), 
  - circular linked lists (in a boss fight)
  - swap nodes (swap platforms to jump to)
  - and a few other medium-difficulty concepts.


# Objects/Entities

- Enemies and their movesets.
- Main Character and their movesets - including their special move, that can eliminate enemies at a range (does not appear until later), a healthbar.
- Bosses and their movesets.
- On-screen buttons for next, previous, and attack.
- On-screen timer for QTE and Boss Fights.
- Platforms.
- Snake Spirit guide and text boxes.
- Announcements. (You win, You lose, Stage Complete, etc.)
- Buttons (Main screen, settings, quit, etc.)

## Core Gameplay Mechanics (Detailed)

- Jump to platforms by solving platform-connection problems (related to linked lists). Traverse a linked list path and be able to choose which platform is next based on which nodes (platforms) are connected to the current node.
- Stealthily execute unaware opponents with action combos. Sneak up on opponents at different parts of the platforms. Be able to perform action combos to take out these opponents. Advancing to more difficult enemies leads you to a boss fight, which is similar in combat, but timed - you lose your turn if the timer runs out on your move. Use your knowledge of linked lists and their connections (links) to link platforms to avoid attacks. Answer questions in a limited amount of time, and finish the boss level to advance to the next topic.
- Incorrect platform connections and not-so-stealthy encounters lead to injury, enough of which can lead to death. As you connect platforms, choosing two in an incorrect order/sequence could cause damage to the health of your player. Additionally, failing to sneak up on opponents can lead to similar injury and loss of health. If player sustains enough damage, it will result in death, causing the player to have to restart the level.
- Traverse the platforms using buttons and delete dangerous spiky platforms to advance. Cross platforms via Previous and Next nodes respectively. Delete dangerous, spiky platforms (ones that would not connect via links) in order to advance past them to more suitable and correctly sequential platforms.

    
## Feedback
**Short Term Feedback**
**VISUAL**
- The player is rewarded with an "Enemy Slain" popup when they kill a regular enemy. They will have an enemy counter to help them see how many they killed. Lastly, once all enemies are killed, they will have a "All enemies slain. Move forward." text popup.
- In the start of the game, the tutorial will be led by a snake spirit that will be very encouraging, saying things like "Good work, you made it to the next platform!" and rewarding the player for their moves. Around the fourth stage, when he fades away, he will reassure the player that they know the most important things to progress forward.
- The stages will be white screens with the stage name and title written on it, so the player is fully aware of their progress.
- On making too many mistakes, the player will die, recieving a black screen that gives them some words of advice based on the reason why they died.

**AUDIO**
- The main character will make a grunting sound when they get hurt, signaling that the player made a mistake, paired with a decreasing healthbar.
- A victorious sound will play on level completion.
- A single slash sound will play, paired with a black screen and a cry from the main character, signaling their death.

**ANIMATION**
- On landing on the last platform, the main character will look back at the level, nod, and walk forth to the next level.
- There will be one "empty area" that the player can run through - signaling a boss battle is incoming and that they are at the final stretch of the gameplay objective of that stage.

**Long Term Feedback**
- A level and stage counter will inform the player of their progression through the game.
- The players deaths (NOT injuries) will be counted to remind them only of continuous mistakes.
- When you win a stage, you get a cutscene into the next stage. When you win the game, you get a more detailed cutscene where the Last Shinobi meets his brother.
- If you make an incorrect connection, you will start at the beginning of the level. The player will recieve a blurb that appears on the top of the screen as to how the character got hurt.
- On completing levels, the player will recieve a congratulatory message.


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

## Aesthetics

The Last Shinobi has an ancient Japanese-themed backstory, so its aesthetic will follow the same. The environment is calm and natural, but tense as you fight the enemies, especially the final boss of each stage. Paired with ambient music, the platforming aspects of the game will be more calm, encouraging players to focus on learning than just playing. 


## Graphical

- Characters List
  - *The Last Shinobi (Takeshi, but name does not appear outside of cutscenes)* - Main and only playable character that executes enemies, moves throughout the level, and leads the story. They are a shadow-like figure sporting a kasa (Japanese straw hat) and commonly seen clothing during the time in an attempt to blend in.
  - *Grunts (Unnamed)* - Main opponents, designed differently in art style based on the stage.
  - *Bosses* - Each boss is named after a Bushido virtue (way of the samurai). They will be shadow-like figures in traditional samurai headwear and clothing.
  - *Akio* - The Last Shinobi's brother, only appears in end cutscene. Frail and pale from his sickness, but happy to see his brother.

- Textures:
  - *Characters* - Characters will mostly be detailed but dark silhouettes.
  - *Cutscenes* - Anime cartoon-like art style/sketchbook-like graphics.
  - *Environment* - Slightly realistic and blurry as you go further, but strong and detailed the more close the plane is to the character. 
  - SEE **STORYBOARDING** FOR VISUAL DETAILS!

- Environment Art/Textures:
  - Each stage has its own background as you approach your destination - from the outskirts of your training grounds, a forest, village outskirts, village, and the final residence of the main boss.
  - The platforms are designed based on their stage - for example, a mud-and-grass platform in the forest versus a stone platform in the training grounds.
  - Some fire effects and particle effects will be added to items like torches and a few fire-based attacks.


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

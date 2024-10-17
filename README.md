# 3D Game Programming Project
CS4555 Game Project for Team 5

November 21st, 2022

Name of Game: Terragrasp

Name of Team: VisualCade

Group Members: Christian Armendariz, Eduardo Cruz, Scott Sun

#### Logline:
You are a human combatant who accepts a mission requiring you to reclaim an enemy-held territory on a distant planet and reestablishing the area’s communication with Earth.

#### Story:
In 2049, a catastrophic dust storm enveloped Phoenix Station, a human colony on Mars. This resulted in all forms of communication with Mars being severed. A series of rescue operations ensued to aid those affected by the dust storm, but masses of extraterrestrial creatures had emerged from the ground of the station, and reinforcements were quickly overwhelmed.

A military operation is conducted in order to reclaim the now decrepit Phoenix Station.

#### Gameplay:
Terragrasp is an action beat ‘em up game, which is played from a third-person perspective. The player is able to move their character around, fight enemies, and collect power ups. Power ups are scattered around the level, and when collected, can provide the player with a temporary advantage against enemies. In addition, the player is able to use abilities to damage multiple enemies or deal more damage to a single enemy. These abilities go into a cooldown after each usage to ensure the player does not become too overpowered. There are different enemy types who will inflict either close-range or long-range attacks against the player. A boss will also hatch from an egg after 2 minutes have passed. To beat the game, the player will have to defeat the enemies and boss.

#### Technology:
There will be many types of enemies with different approaches to defeating the player, requiring different scripts to be created. These scripts would rely on a variable representing the distance between the enemy and the player, since close range enemies would need to check when the distance is very small, while long range enemies would check when the distance is somewhat large. In addition, a navigation mesh agent would have to be attached to our enemies so that they take advantage of the NavMesh component, which is a mesh that helps approximate walkable areas and obstacles via a path finding algorithm provided by the Unity engine. Another type of close range enemy has been created differently with a behavior tree algorithm. This enemy makes decisions by checking the behavior tree from root to nodes.

Our game’s boss is able to attack the player at close and long range depending on the player’s distance. The boss’s long range attack is able to temporarily reduce the player’s movement speed and will enter a second phase when the boss’s health drops to 50%.

There will be power ups that provide a temporary advantage for the player when dealing with a large number of enemies. This will require a script that not only checks when the player has interacted with a power up, but it will also need to modify the player’s attributes for a limited time and then revert these changes.

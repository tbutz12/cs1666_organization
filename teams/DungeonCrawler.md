# CS1666 Team DungeonCrawler

## Canonical game repo URL:

https://github.com/DungeonCrawlerCS1666/DungeonCrawler

## Team Members
* Advanced Topic Subteam 1 (Procedural Generation)
	* Sebastian Marcano-Jimenez
		* Pitt ID: sem203
		* Github Username: sebastian1126
		* Personal Fork URL: https://github.com/sebastian1126/DungeonCrawler
	* Connor Allington
		* Pitt ID: coa18
		* Github Username: callington1
		* Personal Fork URL: https://github.com/callington1/DungeonCrawler
	* Myles Conlon
		* Pitt ID: mac479
		* Github Username: mac479
		* Personal Fork URL: https://github.com/mac479/DungeonCrawler
	* Adam Mattioli
		* Pitt ID: afm45
		* Github Username: amattioli7
		* Personal Fork URL: https://github.com/amattioli7/DungeonCrawler
* Advanced Topic Subteam 2 (Network Multiplayer)
	* Destiny Thompson
		* Pitt ID: dmt67
		* Github Username: DMT67
		* Personal Fork URL: https://github.com/DMT67/DungeonCrawler
	* Zach Stata
		* Pitt ID: zrs17
		* Github Username: zstata
		* Personal Fork URL: https://github.com/zstata/DungeonCrawler
	* Tristin Butz
		* Pitt ID: tmb132
		* Github Username: tbutz12
		* Personal Fork URL: https://github.com/tbutz12/DungeonCrawler
* Advanced Topic Subteam 3 (Game AI)
	* Bryce Ryan
		* Pitt ID: bar68
		* Github Username: BryceRyan
		* Personal Fork URL: https://github.com/BryceRyan/DungeonCrawler
	* Andrew Preston
		* Pitt ID: arp119
		* Github Username: apres123
		* Personal Fork URL: https://github.com/apres123/DungeonCrawler
	* James Bickerstaff
		* Pitt ID: jjb169
		* Github Username: jjb169
		* Personal Fork URL: https://github.com/jjb169/DungeonCrawler
	* Tristan Possessky
		* Pitt ID: tlp64
		* Github Username: tpossessky
		* Personal Fork URL: https://github.com/tpossessky/DungeonCrawler

## Game Description
A high fantasy hack and slash dungeon crawler with the ability to create parties and play with others PvE.  Dungeons will be procedurally generated mazes of rooms that increase in difficulty as the player goes deeper.  The layout will be floor based, and the players advance to the next floor by finding the stairs that are randomly placed somewhere on the map.  The end goal is to reach the bottom/top floor of the dungeon, which will be a "boss room" that will contain a difficult encounter, be it a lot of enemies or a specified boss.  From this the player will get high tier loot that they can then use to take on more difficult dungeons to get even better loot, and so on and so forth.  Loot is procedurally generated and will follow a common/rare/epic/legendary rank system.  Loot can drop randomly from defeated enemies as well as from chests that can be found scattered around the map.  Combat will follow a real time hack and slash format, with players using weapons/skills to deal damage to enemies.  Enemies will each have their own AI and behaviors, as well as a game master AI that will track what enemies are giving the players trouble, what they are doing well against, and dynamically adjust the enemy types, amounts, and locations to ensure a sufficiently difficult experience.
## General Milestones
* Milestone 1 - Game engine
	* System of tracking object placement in the 2D environment
	* Capability to place rooms and hallways and enforce their bounds on objects
	* Character movement within the environment
	* Enemy placement and movement
	* Establish basic combat system of attacking with a sword and being attacked back
* Milestone 2 - Flesh out game
	* Health tracking of all characters
	* Add in ranged combat mechanics
	* Inventory management (Pick item up, drop item, equip item, keep item in inventory, etc)
	* Implement how loot drops
	* Player stats i.e. speed, strength, defense, etc
	* Basic enemy AI that can be elaborated on later
	* Define distinct types of enemies as well as their behaviors - most likely 5-7 different types
	* Add more item and enemy types each with their own features to make them unique
	* Ability to continue the character's progress into the next dungeon
* Milestone 3 - Advanced topic incorporation (Specifics will be below under the subteam's milestones)
	* Procedurally generated floors
		* Implement multiple floor "types", some consisting of 2-3 larger rooms with a few other smaller ones spread around, others being mazes of 8-10 smaller rooms, others a combination of 4-5 smaller rooms with one big room, and others if anything else is thought of
	* Procedurally generated loot
	* Intelligent enemy placement
	* Expanded enemy AI and tactics
	* Party based play with 1-4 people
	* Loot management between people
...

## Advanced Topics

* Procedural Generation
	* Implement ability to algorithmically place rooms, instead of by hand
	* Implement map "collision detection" so rooms do not overlap
	* Establish bounds of the placement algorithm - min/max rooms per floor, size of each floor, min/max distance between rooms, etc
		* Can be different for each floor archetype or a general set of rules
	* Design an algorithm that will plan out rooms in a maze-like configuration (think Pokemon Mystery Dungeon maps)
	* Implement algo and fine tune to give us the correct map look and feel
	* Design a means to randomly generate player level appropriate loot that is randomized
* Network Multiplayer
	* Establish stable peer to peer connection between party members
	* Ensure that players can see each other move around the map accurately and in a synchronized fashion
	* Implement synced up enemies and locations between players
	* Implement combat over network, i.e. 2 players damaging the same enemy at once
	* Implement loot mechanics over network - either instanced or non
* Game AI
	* Create a basic tracking enemy AI so other parts of the game can be tested
	* Implement all of said behaviors in their own separate AI - examples of a few enemies
		* Ranged type that will fire at the players while they are engaged with other enemies, and then run/kite the players when engaged 1 on 1
		* Basic melee grunt utilizing the basic tracking AI, maybe improved a bit depending on the initial quality
		* A knight or gladiator type that will move more intelligently, attempting to dodge attacks (within reason) and fight smarter/less recklessly than just running at the player, while being much tankier than the average enemy
		* Pack mentality or swarming enemy with many of them acting as one to acheive the same goal - example being all attacking the same player at the same time as opposed to just randomly picking one or attacking whoever is closer
		* Hit and run glass cannon, some sort of melee or ranged (or both) character that prioritizes huge damage and staying out of reach.  Will follow the player and try and deal large amounts of damage when they are vulnerable before disappearing again by running away or some other mechanic.  Very low health.
		* We may add more to this list as time goes on if inspiration strikes us, this is just an initial enemy set
	* Game Master AI
		* Implement system to track and understand how the players are dealing with different enemy types
		* Ability to draw conclusions from this info, be it in a ML format or baked into the AI more simply, and place enemies accordingly
		* Ability to update conclusions and make sure that the AI is not fueling its own conclusions (giving more of enemy X leads to even more weight towards enemy X

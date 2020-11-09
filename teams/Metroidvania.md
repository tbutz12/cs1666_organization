# CS1666 Team Metroidvania

## Canonical game repo URL:

https://github.com/ElmaK141/Metroidvania_CS1666

## Team Members
* Physics Engine
	* Joey Weiss
		* Pitt ID: jbw40
		* Github Username: JoeyWeiss
		* Personal Fork URL: https://github.com/JoeyWeiss/Metroidvania_CS1666
	* Emil Kjenstad
		* Pitt ID: emk113
		* Github Username: EmilKjenstad
		* Personal Fork URL:https://github.com/EmilKjenstad/Metroidvania_CS1666
	* Kristofer Elmarsson
		* Pitt ID: kle38
		* Github Username: ElmaK141
		* Personal Fork URL: https://github.com/ElmaK141/Metroidvania_CS1666
	* Adam Buchinsky
		* Pitt ID: asb153
		* Github Username: AlmondDust
		* Personal Fork URL: https://github.com/AlmondDust/Metroidvania_CS1666
		
* Artificial Intelligence
	* Julian Parayil
		* Pitt ID: jtp59
		* Github Username: tgrtgak
		* Personal Fork URL: https://github.com/tgrtgak/Metroidvania_CS1666
	* Giovanni Meiser
		* Pitt ID: gam81
		* Github Username: gam81
		* Personal Fork URL: https://github.com/gam81/Metroidvania_CS1666
	* Joey Valentino
		* Pitt ID: 
		* Github Username: jov34
		* Personal Fork URL: https://github.com/jov34/Metroidvania_CS1666
		
* Procedural Generation
	* Noah Vienneau
		* Pitt ID: nmv28
		* Github Username: nvienneau
		* Personal Fork URL: https://github.com/nvienneau/Metroidvania_CS1666
	* Jordan Bender
		* Pitt ID: jmb416
		* Github Username: benderjm
		* Personal Fork URL: https://github.com/benderjm/Metroidvania_CS1666
	* Zach Hicks
		* Pitt ID: zsh5
		* Github Username: zaryhicks
		* Personal Fork URL: https://github.com/zaryhicks/Metroidvania_CS1666

## Game Description
A metroidvania with a focus on ranged combat and movement. The weapons and gadgets unlocked compliment the movement system and allows for intricate navigation. Sections of proceduraly generated areas branch predesigned locations for a mix of purposefully designed world design and procedurally generated areas inbetween. 

## General Milestones

* Develop a moving prototype
* Implement weaponry (Melee and Ranged)
	* Melee weapon
	* Ranged weapons
* Implement enemy AI
* Implement procedurally generated sections
* Design the world
* Implement boss AI
* Implement quest system
...

## Advanced Topics

* Physics Engine
	* Rigid Body Collision
		* Player character with the environment, enemies, and projectiles
		* Melee weaponry with environment and enemies
		* Projectiles from ranged weaponry on environment and enemies
	* Movement
		* Have gravity at a level which makes movement fun (ligher than Earth)
		* Implement recoil on ranged weaponry and upon impact with melee weaponry
		* Implement grappling with a the ability to hook onto any surface and move in a circular fashion from the point of rotation at an adjustible distance
		* Unique movement options like air dash and double jump
		* Momentum increasing maximum speed after continuous uninterupted directional movement
		
	...
* Artificial Intelligence
	* Implement basic enemy AI
		* Some are basic roamers
		* Some can react to the player's attack by guarding or dodging
		* Enemies will move on a system that will allow them movement no matter how the level is generated
		* Chasers that have similar movement abilities to the player and can hunt down the player 
		* A similar enemy but instead of hunting the player, the player hunts them
	* Implemnt boss AI
		* The boss will be far more intelligent than the basic enemies
		* It will have the ability to strategize and learn throughout the encounter
		* At different health points, it will change "phases"
		
	...
* Procedural Generation 
	* The entire game is not going to be procedurally generated, instead there will be points of premade areas and PG pathways between these premade areas
	* Implement a procedural generation system
	* Make sure all generated levels are playable
		* Can the player reach from point to point with the powerups they have or can access?
	* Create a system that generates levels according to the equipment/powerups the player has
		* The system will have to know where certain key equipments are in the map, which is decided manually, and generate appropriately. 
			* Ex: The pathway from powerup 1 and 2 can generate a pathway that requires powerup 1 but not 2. Shortcuts that require both are allowed as long as there is a way to get from poweup 1 to powerup 2 with just powerup 1.
	...

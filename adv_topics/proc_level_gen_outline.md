# Procedural Level Generation Advanced Topic Presentations

## Presentation I (Oct. 7):
* What is Procedural Generation?
	* Used to create “unique” worlds, levels, loot, encounters
	* Different than Random Generation
	* Commonly uses Noise
* History and Examples
	* Early Use in Gaming\
		* Akalabeth and Rogue
		* Diablo and Daggerfall
	* Graphics / Animation
	* Open World - Worlds
		* Dwarf Fortress
		* Minecraft
		* No Man’s Sky
	* Action - Loot
		* Borderlands
* How does it work?
	* Basics
		* Perlin Noise
	* Algorithms
		* Diamond Square
		* Spelunky Case Study
* Why use Procedural Generation?
	* Pros
		* Smaller file sizes
		* Generate large amounts of content
		* Extra time available for complex gameplay
		* Higher replayability
		* Adjustable Difficulty
	* Cons
		* Complexity of implementation
		* Risk of creating predictable content
		* Loss of Fine Tuned Control
* Applying it to our game
	* Procedurally generated sections connecting premade zones
	* Generate traversable, fun environments appropriate for current loadout
	* Challenge: procedurally generated areas must always have a path that players can traverse with their current gear

## Presentation II (Oct. 21):
# What is Binary Space Partitioning?
* Method for recursively subdividing a space into two convex sets
* History of Binary Space Partitioning
# How does it work?
* Creating the binary tree
* Drawing the rectangles in each leaf node
* Connecting the rectangles with hallways
# What games use BSP?
* Doom (1993)
* Quake (1996)
# Pros
* Good for collision detection and handling
* Easy to visualize with tiles/arrays
* Produces noticeable randomness each time
# Cons
* Generating a BSP tree can be time-consuming/resource intensive
* Can get rather complicated to implement
# How did we implement it?
* Variable parameters
  * Room size
  * Map size
  * Hallway size
  * Tile size
Array integration
SDL_Surface/Rect Usage


## Presentation III (Nov. 2):
* 

## Presentation IV (Nov. 16):
* 


# CS1666 Team SpeedRun

## Canonical game repo URL:

https://github.com/Speedrun-Game-Dev-Pitt-CS1666-Fall-2020/Speedrun

## Team Members
* Advanced Topic Subteam 1 (Physics System)
	* Robert Xu
		* Pitt ID: rox5
		* Github Username: RobertXu09
		* Personal Fork URL: https://github.com/RobertXu09/Speedrun
	* Spencer Miller
		* Pitt ID: sdm74
		* Github Username: spap975
		* Personal Fork URL: https://github.com/spap975/Speedrun
	* Ryan Yang
		* Pitt ID: rcy7
		* Github Username: ruzakiff
		* Personal Fork URL: https://github.com/Ruzakiff/Speedrun
* Advanced Topic Subteam 2 (Procedural Level Generation)
	* Ryan Durkoske
		* Pitt ID: rjd68
		* Github Username: ryandurkoske
		* Personal Fork URL: https://github.com/ryandurkoske/Speedrun
	* Connor Kalina
		* Pitt ID: cjk94
		* Github Username: cjk94
		* Personal Fork URL: https://github.com/cjk94/Speedrun
	* Andrew Francioni
		* Pitt ID: ajf109
		* Github Username: ajf109
		* Personal Fork URL: https://github.com/ajf109/Speedrun
* Advanced Topic Subteam 2 (Networking)
	* Jacob Musone
		* Pitt ID: jpm160
		* Github Username: jmusone
		* Personal Fork URL: https://github.com/jmusone/Speedrun
	* Carter Smith
		* Pitt ID: cas380
		* Github Username: cas380
		* Personal Fork URL: https://github.com/cas380/Speedrun
	* Alexander Pujols
		* Pitt ID: alp203
		* Github Username: alp203
		* Personal Fork URL: https://github.com/alp203/Speedrun
	* Lucas Chronister
		* Pitt ID: lpc17
		* Github Username: lpc17
		* Personal Fork URL: https://github.com/lpc17/Speedrun 

## Game Description
Our game is a 2D platformer in which multiple players race against each other to get to the finish line first. The goal isn't based on high scores or fastest times---this game is a multiplayer platformer race in real time. The concept of the game is a race to the bottom of a cave for treasure, so rather than left-to-right the general direction of the race is from top-to-bottom. Each race will be procedurally generated, with platforms and obstacles placed to create a challenging yet still beatable course. A physics system will promote interactivity between both players with each other and players with the course. An analagous game would be Fun Run, but this game will have unique courses per run so that players will have a unique experience per play of the game.

## General Milestones

* Create a unique, standalone level each time players start a race in the game
* Obstacles will include springtraps that launch players up, rolling/bouncing rocks that knock players around, and slippery terrain that have varying levels of friction. Moving platforms will also exist of course.
* Allow for multiple players (2-4?) to play and interact with each other at the same time
* Create responsive platformer movement (arrow keys and WASD) that is affected by physical interactions with the course and other players
...

## Advanced Topics

* Physics System
	* Players characters will have forces applied on them that reflect how obstacles (springtraps and bouncing balls) and other players bump into them + gravity. 
	* Varying pieces of terrain will apply different levels of friction on players and other kinematic objects (bouncing balls/rocks and potentially other obstacles)
	* The motion of moving obstacles (bouncing balls/rocks) will be governed by physical rules of collisions and gravity
	...
* Procedural Level Generation
	* Implement basic cave generation, with multiple rooms(4+)/layers(2+). The cave would look like an anthill with a single tunnel; players will have to go left, right, down, and sometimes even back up through a tunnel filled with various obstacles. Overall, the goal is for each player to get to the bottom of the "anthill" before the other players. Each run should take at least a minute or two to complete.
	* Coordinate with physics team to make sure the generated course is completable, challenging, and sufficiently unique from previous runs. For example, generated levels should not all have the same room layout (some will go down, far right, then down; some will go left, down, left, up,right then down).
	* Add different biomes/obstacles to terrain. Individual rooms will be themed to have certain types of obstacles---icy floors, rolling rocks, springtraps. Obstacles won't be mixed haphazardly. 
	* Work with Networking team to allow for the ability to save and exchange randomly generated levels to be played again
	...
* Networking
	* Get the server and client working and talking to each other
	* Get at least 4 players on the same server and properly moving on each other's screen
	* Make sure other objects are also synced properly on each other's screen
	* Work with Procedural Level Generation team to allow for the ability to save and exchange randomly generated levels to be played again
	...

# CS1666 Team PuzzleStealth

## Canonical game repo URL:

https://github.com/1666-Puzzle-Stealth/StealthPuzzle

## Team Members
* Advanced Topic Subteam 1: AI Enemies

	* Marko Djurdjevic
		* Pitt ID: mad351
		* Github Username: Markoozy
		* Personal Fork URL: https://github.com/Markoozy/StealthPuzzle

	* Emma Howard
		* Pitt ID: eeh58
		* Github Username: eh0w
		* Personal Fork URL: https://github.com/eh0w/StealthPuzzle

	* Connor Robinette
		* Pitt ID: cjr84
		* Github Username: ConnorRobinette
		* Personal Fork URL: https://github.com/ConnorRobinette/StealthPuzzle

	* Anna Beach
		* Pitt ID: arb223
		* Github Username: arbeach123
		* Personal Fork URL: https://github.com/arbeach123/StealthPuzzle

* Advanced Topic Subteam 2: Network Co-op

	* Turner Halligan
		* Pitt ID: tth16
		* Github Username: turnerhusa
		* Personal Fork URL: https://github.com/turnerhusa/StealthPuzzle

	* Patrick Rhee
		* Pitt ID: psr15
		* Github Username: patrickrhee
		* Personal Fork URL: https://github.com/patrickrhee/StealthPuzzle

	* Andrew Thompson
		* Pitt ID: ant118
		* Github Username: and-thomp
		* Personal Fork URL: https://github.com/and-thomp/StealthPuzzle

* Advanced Topic Subteam 3: Level Generation

	* Chris Godfrey
		* Pitt ID: ctg18
		* Github Username: CGOD737
		* Personal Fork URL: https://github.com/CGOD737/StealthPuzzle.git

	* Celest Hayden
		* Pitt ID: chh147
		* Github Username: celhhayden
		* Personal Fork URL: https://github.com/celhhayden/StealthPuzzle

	* Erik Houseworth
		* Pitt ID: erh100
		* Github Username: altaurus321
		* Personal Fork URL: https://github.com/altaurus321/StealthPuzzle

## Game Description

A co-op puzzle stealth game where one player controls the "Agent" whose job it is to infiltrate a facility and the other player controls the "Hacker" whose job it is to 
hack into various systems in order to assist the Agent. 

The Agent's gameplay will focus on moving around a facility, avoiding or disposing of guards, physically interacting with the environment, giving the Hacker access to 
subsystems, etc.

The Hacker's gameplay will focus around a computer screen that will allow the hacker to see a simplified representation of the facility with icons to click on to access
certain systems such as cameras, doors, computers, security systems of various types, and other electronics. The Hacker's screen can also display documents that may
contain useful information, the location of guards (provided the Hacker has accessed the proper subsystem), and a window for puzzles.

Puzzles will be framed in the context of hacking/infiltrating. Some puzzles will only need to be solved by the Agent (i.e. lockpicking) and others only by the Hacker (i.e. password cracking).
Some puzzles will require the Agent and the Hacker to work together and exchange information in order to succeed.

Objectives for the team to complete will range from extracting VIPs, stealing sensitive information, assassinating a target, etc.

## General Milestones

* Agent can move around in environment and is stopped by walls and obstacles.
* Hacker can see simplified representation of facility in one window
* Hacker has multiple windows
* Hacker can access subsystems (Cameras, computers, security lasers, guard trackers, etc.)
* Agent can interact with systems (lockpick doors, etc.)
* Agent can give Hacker access to systems
* Both players have puzzles to solve to access systems (word search for password, torn document puzzle, simon says, scrambled wires, lockpicking)
* Collaborative puzzles (Hacker/Agent has information that the other doesn't, must share information to solve, like a maze where only the hacker sees the obstacles and must guide Agent through)
* Agent can interact with guards (KO, kill, etc).

...

## Advanced Topics

* AI
    
    * Stationary cameras/gun turrets.
    * Guards on set patrol paths with FOV
    * Guards respond to perceived threats and alarms
    * Guards dynamically form new patrol paths in areas where Agent was detected
    * Guards with different behaviors and states (Alert, Lazy, Normal, Underpaid fat security guard vs Highly paid merc)
    ...
* Network/Co-op

    * Depending on the host, Hacker and Agent can affect each other's games.
    * Low latency collaborative real time synchronous puzzles (If players need to press things at the same time)
    * Server that hosts levels and stores player times and stats.
    * 
    ...
* Level Generation

    * Grid based level creation where a particular object inhabits one box (doors, walls, windows) anywhere from 20x20 to 100x100
    * Generate random objectives based on rooms
    * Generate random guard patrol routes
    * Generate random subsystem and local network layouts.
    * Generate random puzzles

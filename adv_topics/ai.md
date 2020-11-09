# AI Advanced Topic Presentations

## Presentation I (Oct. 14):
* What is Artificial Intelligence?
    - Definition
    - Different Types
    - Simple explanation of uses, in gaming and otherwise

* History of Artificial Intelligence
    - First AI Program
    - First game(s) to feature AI
    - First Machine Learning

* Some Examples of AI
    - Finite State Machine
    - Monte Carlo Search Tree
    
* How will we implement it in our game?
    - Security guards adapting
    - Different levels of guard intensity/activity
    - Fear Factor (react based on fear of agent actions)
    
* (semi)Modern Examples:
    - Halo, Fear, Arkham Trilogy, Shadow of War, Alien: Isolation, Sims

## Presentation II (Oct. 26):
* Goals for AI in a Metroidvania
    - Whittle down the player
    - Guard extra areas
    - In conjunction with level design, provide a difficult gauntlet for the player
* Concepts to emulate
    - “Rigid path” enemies (gordos, medusa heads from castlevania)
    - Hp gates
    - Reactionary behavior and adaptation
    - Modification via difficulty settings 
    - Arbitrary boss resources/cooldowns to prevent predictable or unfair move-spamming
* Dynamic principles
    - Behavior selection
        - Deciding between rushing the player or waiting for the player to overextend
* Planned implementation
    - Enemy behavior
        - Unintelligent horde combat
        - Gimmicky triggers and spawns
    - Boss behavior
    - Group vs solo attacking
    - Varied pathing
* Example of Metroidvania A.I.
    - Shovel Knight
        - Difficult bosses, enemies used as springboards

	

## Presentation III (Nov. 9):
* Dungeon Crawler AI Use Cases and goals
   - Make the game interesting - other teams provide the bedrock, we provide the flair
   - Have a set of 5 enemies with diverse behaviors that can antagonize the player in different ways in conjunction with one another
   - Monitor the player experience and adjust difficulty dynamically
* Techniques used
   - Enemies
      - Heatmapping enemy pressure to make decisions
         - Specific implementation - matrix of doubles
         - Image blur algorithm
   - AI Data Structure
      - Decision Tree
   - Pathfinding - in depth A*
   - Important Methods
* Game Master AI
   - Compare an average damage dealt per character to the actual damage dealt, determine difficulty by health
   - Benchmarking each enemy in different situations to determine avg damage output
      - Comparing instantiated run’s Z scores vs benchmarked data
* Enemy types and implementations
   - Grunt
      - Simple chase on sight, nothing too special to talk about
   - Archer
      - Kiting vs stand still modes and deciding between them
   - Assassin
      - Hit and run from the shadows - not implemented yet
   - Knight
      - Tanky brute that protects the smaller units - not implemented yet
   - Swarmer
      - Teamwork based surrounding unit
      - Pack mentality code





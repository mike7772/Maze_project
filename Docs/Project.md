Getting Started
STEP 1: Start the application server
Start by running api.py at ./Web/api.py

STEP 2: Start the game
Then run main.py at ./Maze/main.py

STEP 3: Play the game
Game ruleset:

The game will request a name. Optional (Defaults to "GUEST")
Controls with the arrow keys.
Crossing a loot item will automatically collect it and display the number of items in the backpack.
The player must collect all loot items before reaching the exit otherwise they lose.
STEP 4: Repeat and compete
When the game ends, replay by running ./Maze/main.py again.
Scores are posted http://localhost:``/

Gameplay and Features
Start screen:
Requests the player's name. Optional (Defaults to 'GUEST')
Shows previous players' high scores.

Press ENTER to continue to the game screen

Game screen:
Player controls:

Arrow keys to move
ESCAPE to exit
Map

Cannot pass through brick walls.
All coins are placed randomly, and must be picked up before using the exit
Coins and backpack

Player must collect all 4 coins before reaching the exit in order to win the game!
Number of coins collected in the player's backpack is shown in the top left corner of the screen.
Timer

Player muct complete the maze before the timer runs out, otherwise they lose the game.
The time it takes for the player to complete the maze is measured to calculate a player score.
Scores
High scores are accessible by a web browser at http://localhost:`/. Player scores are saved as ./Web/scores.json`

The score is the time it took a player to successfully complete the game. The less time, the better the score. For example a game that took 12 seconds to complete gets a score of 12, better than a game that took 15 seconds to complete. Failed games are given a default score of 1000

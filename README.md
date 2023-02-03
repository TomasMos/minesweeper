# minesweeper

## This game was developed as part of my CS50AI course from Harvard. On the frontend, pygame is used to create the graphics and GUI. The backend enables a human to make moves and calculates the optimum move for an AI to play. The AI algorithm employed is based on a set of logical statements about the board. For example, if a cell is known to have the value of 0 (indicating that there are no mines immediately next to it) then the knownledge base of the AI is updated with information to say that all the neighbouring cells are 'safe'. To add to this, the logical statements can be combined, to infer knowledge about cells outside of the immediately obvious neighbours. An example is shown below. 


### Gamplay

#### This is the home page, detailing how to play the game.

![Home Page](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/home.PNG)

#### As with normal minesweeper, the board begins blank and a player needs to make an initial guess, here the AI has guessed and has revealed a cell with a value of 0. This will update the AI's knowledge base with the information of this cell's value, and that the neighbouring cells are 'safe'.

![Play as X](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/initial_guess.PNG)

#### Sometimes, the initial guess will hit a mine, and the game will be over.

![Make suboptimal moves, the AI will win](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/bad_guess.PNG)

#### Here, it took a few guesses for the AI to find a cell with a value of 0, only now will the AI have the knowledge of where to safely move. It operates exactly the same as a human player would

![Play as O](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/few_guesses.PNG)

#### The AI, capitalized on the known 'safe' cells by revealing those cells closest to the initial 0-valued cell. But, highlighted in yellow is an example of inference made by the AI. This cell with the value 2 is the most recent move by the AI, and was not a guess (I know because in the terminal it prints whether the AI is guessing or making a safe move). This move is based on two separate logical statements, which have been combined to create a third logical statement about the highlighted cell, that it is 'safe'. This is most definitely not a human move.

![The AI has cornered me with a catch-22](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/AI%20move.PNG)

#### Below is an example of the AI winning the game.

![The AI has won](https://raw.githubusercontent.com/TomasMos/minesweeper/main/screenshots/won.PNG)

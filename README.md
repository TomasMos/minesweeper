# minesweeper

## This game was developed as part of my CS50AI course from Harvard. On the frontend, pygame is used to create the graphics and GUI. The backend enables a human to make moves and calculates the optimum move for an AI to play. The AI algorithm employed is based on a set of logical statements about the board. For example, if a cell is known to have the value of 0 (indicating that there are no mines immediately next to it) then the knownledge base of the AI is updated with information to say that all the neighbouring cells are 'safe'. To add to this, the logical statements can be combined, to infer knowledge about cells outside of the immediately obvious neighbours. An example is shown below. 


### Gamplay

#### This is the home page, where a human can choose to play as X or O, if one chooses O they play second, X goes first.

![Home Page](https://raw.githubusercontent.com/TomasMos/tictactoe/main/Home.PNG)

#### I chose to play as X and the AI chose the top left corner cell as O.

![Play as X](https://raw.githubusercontent.com/TomasMos/tictactoe/main/X_1.PNG)

#### After I played a series of suboptimal moves, the AI has won.

![Make suboptimal moves, the AI will win](https://raw.githubusercontent.com/TomasMos/tictactoe/main/X_win.PNG)

#### This is the AI playing as X.

![Play as O](https://raw.githubusercontent.com/TomasMos/tictactoe/main/O_1.PNG)

#### The AI has cornered me with a catch-22, where I cannot prevent losing as there are two winning moves for the AI.

![The AI has cornered me with a catch-22](https://raw.githubusercontent.com/TomasMos/tictactoe/main/O_2.PNG)

#### The AI wins again.

![The AI has won](https://raw.githubusercontent.com/TomasMos/tictactoe/main/O_win.PNG)

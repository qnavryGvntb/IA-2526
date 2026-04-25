# CC2006 Artificial Intelligence

## Pop Out: The Game
_PopOut_ is a variant of Connect-4. It starts the same as traditional gameplay, with an empty board
and players alternating turns placing their own coloured discs into the board. During each turn, a
player can either add another disc from the top, or if one has any discs of their own colour on the
bottom row, remove (or “pop out”) a disc of one’s own colour from the bottom. Popping a disc out
from the bottom drops every disc above it down one space, changing their relationship with the rest
of the board and changing the possibilities for a connection. The first player to connect four of their
discs horizontally, vertically, or diagonally wins the game.
_PopOut_ differs from Connect-4 by the introduction of pop moves and three additional rules to
handle draws and wins. These three rules are needed to remove ambiguity about what the result of
the game is:
- The first rule deals with simultaneous four-in-rows. If a pop move creates four-in-rows for both
players, the player who made the pop move is declared a winner and the other player’s four-in-row
is ignored.
- The second rule allows the game to be drawn if the board is full. In such a case, the player to
move decides whether he wants to make a pop move or end the game as a draw.
- The third rule handles repetitions. If the same state is repeated three times, either player can
declare the game drawn.

## Game Interface
The interface is the following:
```
+-------+
|       |
|       |
|       |
|       |
|X  O XO|
|X OXOXO|
+-------+
|0123456|
+-------+
```
After X makes a move, the computer takes this new board and uses one of the two algorithms to
be implemented. When the computer finishes choosing the best move among the possible ones, it will
then exhibit a new board with the computer’s move, and wait for the human to play.
Your implementation will need to support the following three game scenarios:
1. human vs. human
2. human vs. computer
3. computer vs. computer (2 different algorithms)

## Work to develop
### Monte Carlo Tree Search
TODO

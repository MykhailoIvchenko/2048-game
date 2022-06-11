1. The project implements game 2048 for desctop. The game is implemented using plane JS.
  The game field is 4 x 4
  Each cell can be empty or contain one of the numbers: 2, 4, 8 ... 2^n
  The player can move cells with keyboard arrows
  All the numbers can be moved in the selected direction until all empty cells are filled in
    - 2 equal cells merge into a doubled number
    - The merged cell can’t be merged twice during one move
  The move is possible if at least one cell is changed after the move
  After move 2 or 4 appears in a random empty cell. 4 probability is 10%
  When 2048 value is displayed in any cell, win message will be shown.
  The `game over` message will be shown if there are no more available moves.
  Start message hides when game starts.
  The `Start` button changes to `Restart` after the first move.
  In each move the score increases by the sum of all merged cells.

  The game implementation is based on a matrix displaying the game field. The matrix changes on every move and method render()
  draws the game field using this matrix. On each move there are some checks:
  1) if the movement in the caused direction possible (if not, nothing happens, and you should push to make move);
  2) if the win number (2048) was received  (if so, the game is over and a corresponding message will appear)
  3) if the game can be continued after new 2 or 4 appearance (if not, the game is over a corresponding message will appear);

2. Technologies stack: HTML5, CSS3, BEM, SASS (I was provided with ready markup and SCSS), JS.

3. Preview link: https:/mykhailoivchenko.github.io/2048-game/

4. The prototype of the game is here: https://play2048.co/

5. Click start button to start new game. Restart makes the same but during the active game.
Use arrows keys on the keyboard to move cells.

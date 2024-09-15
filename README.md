# Amateur-TicTacToe

If we have a 3x3 grid, then we need 3-in-a-row for a winner

[1,1,0] [1,2,0] [1,3,0] <br>
[2,1,0] [2,2,0] [2,3,0] <br>
[3,1,0] [3,2,0] [3,3,0] <be>

Each spot will be initialized as an array with [ row , column , condition ]

## functions considered

After each turn:
* Are there any winners?
* Are all the spots filled?

Before BOT turn:
* Do I have win condition available?
   * No - does PlayerOne have Win condition?
      * Yes - Stop PlayerOne Win Condition
      * No - Pick any available spot
   * Yes - Can the BOT win this turn?
      * Yes - Pick the spot and win the game
      * No - Does PlayerOne have a Win condition?
         * Yes - Stop PlayerOne Win Condition
         * No - Pick a winning strategy

In these available series of conditions we should consider functions:
* Stop playerOne from winning
* Check for available win conditions (player and bot)

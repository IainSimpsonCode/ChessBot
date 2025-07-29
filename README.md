# ChessBot

```mermaid
graph TD;
  Constants-->ClickableLabel;
  Constants-->Pieces;
  ClickableLabel-->Display;
  Constants-->Board;
  Display-->Game;
  Board-->Game;
  Pieces-->Pawn;
  Pieces-->King;
  Pieces-->Queen;
  Pieces-->Bishop;
  Pieces-->Knight;
  Pieces-->Rook;
  Pawn-->Game;
  King-->Game;
  Queen-->Game;
  Knight-->Game;
  Bishop-->Game;
  Rook-->Game;
  Board-->Display;
```

## Board
Stores the postition of the pieces based on an FEN string provided to the constructor from the parent game.
Can evaluate the position and return a value to determine who is in a more favourable position.

## Game

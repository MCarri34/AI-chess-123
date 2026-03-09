# Chess AI Project

This project is a playable chess game with an AI opponent. The board is initialized using a FEN string and all pieces follow the correct chess movement rules. The player controls the white pieces and the AI controls the black pieces. Moves alternate turn by turn just like a normal two-player chess game, and pieces can capture each other according to the rules.

The AI is implemented using the **Negamax algorithm with alpha-beta pruning**. Negamax searches possible moves and evaluates the board to decide which move is best. Alpha-beta pruning improves performance by cutting off branches of the search tree that cannot produce a better move. The AI searches to a **minimum depth of 3**, allowing it to look ahead multiple turns instead of choosing random moves.

The board evaluation function scores the position based on the material value of pieces (pawns, knights, bishops, rooks, queens, and kings). White pieces contribute positive values and black pieces contribute negative values, allowing the AI to determine which board state is better. This evaluation allows the AI to prioritize captures and stronger positions, making it play noticeably better than a random move generator.

## Gameplay Video

Video of me playing against the AI:

[INSERT VIDEO LINK HERE]

## Features Implemented

* Chess board initialized using FEN
* All chess pieces move according to the rules
* Turn-based gameplay between player and AI
* Move generation for all pieces
* Negamax AI algorithm
* Alpha-beta pruning for faster search
* Minimum search depth of 3
* Board evaluation based on piece values
* AI plays stronger than random moves

## Notes

When the AI moves, it reloads the piece it moved, but it still does the legal movement of said piece.
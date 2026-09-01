# AI Chess Engine - C++ & Raylib

A fully featured, 100% rules-compliant Chess Engine written from scratch in C++. 
The game features a custom minimax AI and a beautiful, minimalist graphical user interface powered by Raylib.

## Features

- **Strict Chess Logic**: Fully implements all standard chess rules, including pseudo-legal and legal move validation.
- **Check & Checkmate Detection**: The engine evaluates board states to prevent illegal moves and correctly detects Checkmate and Stalemate scenarios.
- **Special Moves Supported**:
  - **Castling**: Supported for both Kingside and Queenside (provided paths are clear and squares are unattacked).
  - **En Passant**: Accurately tracks pawn double-steps to allow diagonal captures on the subsequent turn.
  - **Pawn Promotion**: Features an interactive UI popup to select a promotion piece (Queen, Rook, Bishop, Knight) when a pawn reaches the 8th rank.
- **Undo System**: A built-in "UNDO" button allows you to safely rewind the game state, restoring captured pieces and reverting both player and AI moves.
- **Custom AI**: Features a custom-built Minimax algorithm (default depth: 4) using alpha-beta pruning and positional piece-square tables (heuristics) to calculate optimal moves.

## How to Play (Windows)

1. Ensure you have MinGW installed on your machine.
2. The repository includes a `build_gui.bat` script that compiles the engine using the included Raylib source files.
3. Simply double-click `build_gui.bat` or run it from your terminal:
   ```cmd
   .\build_gui.bat
   ```
4. The game window will open automatically upon successful compilation. 

## Controls
- **Mouse Left-Click**: Select a piece (highlights yellow) and click a valid destination square to move.
- **Undo**: Click the UNDO button in the bottom left corner at any time during your turn to rewind the previous move.

---
*Built as a showcase for C++ game logic and minimax algorithm implementations.*

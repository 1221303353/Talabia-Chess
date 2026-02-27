# Overview

This project is a GUI-based Java implementation of Talabia Chess, a two-player strategy board game played on a 7×6 board. The game introduces unique movement rules and a transformation mechanic that differentiates it from traditional chess.

This project emphasizes:
- Proper Object-Oriented Design
- Implementation of the Model-View-Controller (MVC) architecture
- Use of appropriate Design Patterns
- GUI-based interaction
- Save and load functionality

# Contributors
| Name | Student ID |
|---|---|
| Abdullah bin Kamaruddin | 1211202025 |
| Muhammad Amir Farid Bin Ahsan Nudin | 1221303353 |
| Afiezar Ilyaz | 1211200107 |
| Shaheendra Sarvesh | 1181101878 |
| Parthasarathy A/L Raman | 1191102837 |

# Game Pieces & Movement Rules
1. Point
  - Moves forward 1 or 2 steps
  - Cannot skip over pieces
  - When reaching the end of the board, it reverses direction

2. Hourglass
  - Moves in a 3×2 L-shape (like a knight in traditional chess)
  - Only piece that can skip over other pieces

3. Time
  - Moves diagonally
  - Can move any distance
  - Cannot skip over pieces

4. Plus
  - Moves horizontally and vertically
  - Can move any distance
  - Cannot skip over pieces

5. Sun
  - Moves one step in any direction
  - The game ends when the Sun is captured

## Special Transformation Rule
After every 2 turns (1 Yellow move + 1 Blue move = 1 turn):
  - All Time pieces transform into Plus
  - All Plus pieces transform into Time

# MVC Architecture
1. Model
  - Contains all game logic
  - Piece movement rules
  - Turn handling
  - Transformation logic
  - Win condition detection
  - Save/load game logic

2. View
  - GUI components
  - Board rendering
  - Resizable window support
  - Screen flipping per player turn

3. Controller
  - Handles user input
  - Communicates between Model and View
  - No game logic inside controller or view

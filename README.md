# Connect 4 Game - MATLAB

A two-player Connect 4 game implementation in MATLAB with graphical interface using the simpleGameEngine.

## Features

- Interactive 6x7 game board with visual display
- Splash screen menu with start option
- Two-player gameplay (Red vs Yellow)
- Command line input for column selection
- Win detection for horizontal, vertical, and diagonal connections
- Post-game menu with options to restart or exit
- Automated disc placement with gravity simulation

## Requirements

- MATLAB (R2019b or later recommended)
- simpleGameEngine library
- Required sprite sheets:
  - `spritesheet.png` (33x33 sprites for game pieces)
  - `spritesheetC.png` (33x33 sprites for menu)

## Installation

1. Clone this repository
2. Ensure `simpleGameEngine.m` is in your MATLAB path
3. Place the required sprite sheets in the same directory as the game file
4. Run `Connect_4.m` in MATLAB

## How to Play

1. Run the script to see the splash screen
2. Click to start the game
3. Player 1 (Red) goes first
4. Enter a column number (1-7) in the command window to drop your disc
5. Discs fall to the lowest available position in the selected column
6. Players alternate turns
7. First player to connect 4 discs horizontally, vertically, or diagonally wins
8. After a win, choose to play again or exit

## Game Rules

- Board size: 6 rows × 7 columns
- Players take turns dropping colored discs into columns
- Discs fall straight down and occupy the lowest available space
- Win by connecting four discs in a row (horizontal, vertical, or diagonal)
- Column must have available space to place a disc

## Code Structure

### Main Components
- **Board initialization**: 6×7 matrix representing game state
- **Game loop**: Handles turn-based gameplay and input validation
- **Win detection**: `checkWin()` function checks all possible winning combinations
- **Menu system**: Start screen and post-game options

### Win Detection Algorithm
The `checkWin()` function checks for four consecutive discs in:
- Horizontal lines (left to right)
- Vertical lines (top to bottom)
- Diagonal lines (both directions)

## Screenshots

(Add screenshots of your game here)

## Known Issues

- Game requires manual column input via command window rather than mouse clicks on the board

## Future Improvements

- Add mouse-click column selection
- Implement tie detection when board is full
- Add sound effects
- Create AI opponent option

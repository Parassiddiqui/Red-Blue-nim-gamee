

# Red-Blue Nim Game

This repository contains a Python implementation of the Red-Blue Nim Game. The game can be played in two modes: **Standard** and **Misère**. Players take turns removing red and/or blue marbles, and the player who takes the last marble wins (or loses, depending on the game version).

## Features

- **Two versions** of the game: Standard and Misère.
- **Human vs Computer**: The human player can compete against a computer opponent.
- The computer uses the **minimax algorithm with alpha-beta pruning** to determine its moves.
- **Adjustable difficulty**: You can modify the depth of the minimax algorithm to make the computer easier or harder to beat.

## Game Rules

1. Players take turns to remove at least one red or blue marble (or both) from the pile.
2. **Standard version**: The player who takes the last marble wins.
3. **Misère version**: The player who takes the last marble loses.

## How to Play

1. **Enter the number of red and blue marbles** at the start of the game.
2. **Choose the version** you want to play:
   - `standard`: The player who takes the last marble wins.
   - `misere`: The player who takes the last marble loses.
3. **Decide who plays first**: The human or the computer.
4. The game will alternate turns between the human and the computer until all marbles are taken, at which point a winner will be declared.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/red-blue-nim-game.git
   cd red-blue-nim-game
   ```

2. Make sure you have Python installed on your system. You can check by running:
   ```bash
   python --version
   ```

3. Run the game:
   ```bash
   python red_blue_nim_game.py
   ```

## Usage

When you run the game, you'll be prompted to enter several values:
- The number of red and blue marbles.
- The version of the game (`standard` or `misere`).
- Who plays first (`human` or `computer`).

Example input:
```
Enter the number of red marbles: 5
Enter the number of blue marbles: 4
Enter the game version (standard/misere): standard
Who plays first (human/computer): human
```

The game will then alternate between the human and computer players until a winner is determined.

## Code Explanation

The game uses the **minimax algorithm** with **alpha-beta pruning** to calculate the best moves for the computer. Here's a high-level breakdown of the key components:

- **RedBlueNimGame class**: This class represents the game and its state. It includes methods to:
  - Display the current state of the game.
  - Handle human and computer moves.
  - Implement the minimax algorithm for the computer to decide its moves.
  - Check if the game is over and calculate the winner.

- **play_game function**: This function runs the main game loop, switching between human and computer players.

## Customization

You can adjust the **depth** of the minimax algorithm to make the game more or less challenging for the computer. This can be done by changing the `depth` parameter in the code. A larger depth makes the computer smarter but slower.


# Capture the Flag - Haskell AI Game

This project is an implementation of a **Capture the Flag** game AI using Haskell. The game features a two-player turn-based strategy where a human player competes against the computer to either capture the opponent's flag or immobilize all opponent pieces. The project leverages **Minimax** search with a **static evaluation function** to determine optimal moves for the computer player, enabling competitive gameplay against the human player.

## Features
- **Game Mechanics**: Players control pawns and a flag on a grid-based board, with specific winning conditions:
  - Capturing the opponent’s flag.
  - Blocking all of the opponent's pawns.
  - Moving one’s flag past all opponent pawns.
- **Minimax AI with Depth Control**: The computer player uses the Minimax algorithm to simulate and evaluate potential moves up to a specified depth, ensuring competitive gameplay.
- **Static Board Evaluation**: The AI evaluates board states with a custom scoring function to determine the value of each position based on criteria like pawn count, flag positioning, and potential threats.
- **Human-Computer Interaction**: The game includes an interactive command-line interface allowing a human player to make moves against the AI, with prompts guiding the gameplay experience.

## How It Works
1. **Static Evaluation**: A board evaluation function scores each state by checking win/loss conditions, piece positioning, and other custom rules. 
2. **Minimax Search**: The AI simulates both players' moves up to a certain depth and chooses the move that maximizes its advantage.
3. **Move Validation**: The game ensures valid moves and prevents repeating positions by maintaining a history of board states, avoiding cycles during gameplay.
4. **Game Interaction**: The human player is prompted to enter coordinates for moves, while the AI’s responses are calculated based on Minimax evaluations.

## Usage
1. **Installation**: Clone the repository and load the project in GHCi or your preferred Haskell environment.
2. **Starting the Game**: Run the `playGame` function to initiate a game session against the AI.
3. **Making Moves**: Enter your move coordinates as prompted. The AI will respond with its move, and the game will continue until a win condition is reached.

## Requirements
- Haskell (GHC) for compiling and running the project.

---

Feel free to copy and paste this into your `README.md` file. Let me know if you'd like any further customization!

# Tic Tac Toe Game in C++

This is a simple implementation of the classic Tic Tac Toe game in C++. The game provides users with three choices in the menu:

1. **Play With User:** Allows two players to take turns on the same computer.
2. **Play With AI:** Implements the Minimax algorithm for a challenging AI opponent.
0. **Exit Game:** Terminates the game.

## How to Play

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/21Sandesh/TicTacToe.git

2. **Compile and Run**
   ```g++ -o TicTacToeGame TicTacToeGame.cpp```
   ```./TicTacToeGame```

3. **Choose Game Mode**
   Enter 1 to play with another user.
   Enter 2 to play against the AI.
   Enter 0 to exit the game.

## AI Implementation
   The AI is Based Upon Minimax Algorithm. The Minimax algorithm is a decision-making algorithm commonly used in two-player turn-based games, where the goal is to find the optimal move that leads to the best possible outcome.

### How Minimax Works:
1. Recursive Tree Search:
   The algorithm constructs a game tree that represents all possible moves and outcomes, starting from the current game state. Nodes in the tree represent different game states, and edges represent possible moves.
2. Minimizing and Maximizing Players:
   The algorithm assumes two players: a maximizing player (usually the AI) and a minimizing player (the opponent or the user). The maximizing player aims to choose moves that lead to the highest possible score, while the minimizing player aims to choose moves that lead to the lowest possible score.
3. Scoring Function:
   Each leaf node in the tree is assigned a score based on the current state of the game. The score is calculated using a heuristic function that evaluates the desirability of that particular game state for the maximizing player.
4. Backtracking:
   The algorithm backtracks from the leaf nodes, propagating the scores up the tree. At each level, the maximizing player selects the move with the highest score, and the minimizing player selects the move with the lowest score.
5. Optimal Move:
   The algorithm ultimately determines the optimal move for the maximizing player by selecting the move that leads to the highest score at the root level of the tree.
   
### Significance in Tic Tac Toe:
In the context of Tic Tac Toe, the Minimax algorithm ensures that the AI opponent always makes the best possible move, making it unbeatable if both players play optimally. The algorithm is particularly effective for games with a finite number of possible states, making it suitable for the relatively simple decision tree of Tic Tac Toe.

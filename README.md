♟️ Omega Chess vs. Smart AI
A high-performance, browser-based implementation of Omega Chess, featuring a custom-built AI engine using the Minimax algorithm with Alpha-Beta pruning.
Omega Chess is a professional chess variant played on a 12 \times 12 board, introducing two powerful new pieces: the Champion and the Wizard.
🚀 Features
 * Advanced AI Engine:
   * Minimax Algorithm: Simulates future moves to make optimal decisions.
   * Alpha-Beta Pruning: Optimizes search speed by skipping irrelevant branches.
   * Piece-Square Tables: The AI understands positional value (controlling the center, king safety).
 * Selectable Difficulty: Toggle AI depth between Easy (Depth 1), Medium (Depth 2), and Hard (Depth 3).
 * Move History & Undo: Step back through the game with a functional Undo system.
 * Responsive UI: Fully responsive design with touch-optimized controls and centered Unicode piece rendering.
 * Zero Dependencies: Pure HTML5/CSS3/JavaScript. No installation or servers required.
📜 Movement Logic & Piece Guide
Omega Chess follows standard chess rules with the following specific additions for the 12 \times 12 environment:
☖ The Champion
The Champion is a "leaper" and a "stepper." It is a versatile defensive and offensive unit.
 * The Jump: Jumps exactly two squares away in any direction: orthogonally (up, down, left, right) or diagonally. It ignores any pieces in between.
 * The Step: Moves exactly one square orthogonally (forward, backward, left, or right). It cannot move one square diagonally.
☾ The Wizard
The Wizard is a color-bound piece and functions as a specialized "long" leaper.
 * The Jump: Moves in a 1 \times 3 or 3 \times 1 "L" shape (an extended Knight's move).
 * The Step: Moves exactly one square diagonally in any direction. It cannot move one square orthogonally.
 * Wizard Squares: The only piece that can occupy the four 1 \times 1 corner squares at the start of the game.
♟️ The Pawn (Triple Jump)
To navigate the larger board, pawns are more mobile:
 * Initial Move: A pawn on its starting rank can move one, two, or three squares forward.
 * En Passant: If a pawn moves 2 or 3 squares to avoid capture, it can be captured "in passing" on any square it bypassed.
🛠️ Installation & Usage
 * Clone the repository:
   git clone https://github.com/yourusername/omega-chess-ai.git

 * Run the game:
   Simply open index.html in any modern web browser (Chrome, Firefox, Safari, Edge).
🧠 AI Evaluation Logic
The engine calculates the best move by maximizing the following formula:

| Piece | Value |
|---|---|
| Pawn | 100 |
| Knight / Bishop | 320–330 |
| Wizard | 350 |
| Champion | 450 |
| Rook | 500 |
| Queen | 900 |
| King | 20,000 |
📄 License
Distributed under the MIT License. See LICENSE for more information.
Would you like me to generate the LICENSE file text or a .gitignore file for your project?



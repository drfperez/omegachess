## Omega Chess Game


A modern implementation of Omega Chess with 4 different AI difficulty levels, featuring unique pieces and a 10x10 board with corner wizard squares.

# 🎮 Live Demo

Play Omega Chess Online (https://drfperez.github.io/omega/)

# 📋 Table of Contents

· Features
· Game Rules
· AI Levels
· How to Play
· Installation
· Technical Details
· Future Improvements
· Contributing
· License

# ✨ Features

· Complete Omega Chess Implementation: Full rules with all special pieces
· 4 AI Difficulty Levels: From beginner-friendly to expert challenge
· Modern UI: Clean, responsive design with visual feedback
· Real-time Game State: Visual indicators for moves, captures, and special rules
· Interactive Tutorial: Built-in help system
· Cross-platform: Works on desktop and mobile browsers

# 🎲 Game Rules

Board Setup

· Main Board: 10x10 chess board
· Corner Squares: 4 wizard squares in each corner
· Pieces: Standard chess pieces plus two new Omega Chess pieces

Special Pieces

Champion (☖/☗)

· Moves 1 square orthogonally (like a King but without diagonals)
· AND jumps 2 squares in any direction (orthogonal or diagonal)
· Combines Wazir (1-step orthogonal) and Dabbaba/Alfil (2-step jumps)

Wizard (☾/☽)

· Color-bound leaper (can only move to squares of the same color it starts on)
· Moves 1 square diagonally
· AND jumps (1,3) or (3,1) squares (like a (1,3) leaper)
· Starts in the corner wizard squares

Pawn Special Rules

· First move: Can move 1, 2, OR 3 squares forward!
· En Passant: Available after double or triple pawn moves
· Promotion: Pawns promote to Queen when reaching the opposite back rank

Standard Chess Rules

· All standard chess rules apply
· Castling is available (though not explicitly implemented in current version)
· Check and checkmate detection (planned for future versions)

# 🤖 AI Levels

The game features 4 distinct AI difficulty levels:

1. Easy (Random)

· Makes completely random legal moves
· Perfect for learning the game mechanics
· No strategic thinking

2. Medium (Basic Strategy)

· Prefers capturing pieces
· Develops pieces toward the center
· Avoids moving pieces into immediate danger
· Basic positional understanding

3. Hard (Advanced)

· Evaluates piece values (Pawn=1, Knight/Bishop=3, Rook=5, Queen=9)
· Considers piece mobility and center control
· Uses 1-ply look-ahead (considers immediate consequences)
· Good challenge for intermediate players

4. Very Hard (Expert)

· Alpha-Beta Pruning algorithm with 3-ply search depth
· Sophisticated position evaluation:
  · Piece-specific position tables
  · Pawn structure analysis (connected pawns, passed pawns)
  · King safety evaluation
  · Mobility and development bonuses
· Provides strong challenge for experienced players
· Note: May think for a moment before moving

# 🎯 How to Play

Starting a Game

1. Open index.html in your web browser
2. Select your preferred AI difficulty level
3. The game begins with White (you) to move

Controls

· Click on a white piece to select it
· Green dots show possible moves
· Red borders show possible captures
· Click on a destination square to move
· The AI (Black) will move automatically

Game Interface

· Status Display: Shows whose turn it is and current AI level
· Control Buttons:
  · New Game: Restarts with current AI level
  · Change AI Level: Opens difficulty selection
  · Help: Shows game rules and instructions
  · Debug: Toggles debug information (for developers)

# 💻 Installation

Option 1: Local Play

1. Download the index.html file
2. Open it in any modern web browser
3. No additional installation required!

Option 2: Web Hosting

1. Upload the index.html file to any web server
2. Access via your server's URL
3. The game works as a single HTML file

Option 3: GitHub Pages

1. Fork this repository
2. Enable GitHub Pages in repository settings
3. Access at https://your-username.github.io/repository-name

# 🔧 Technical Details

Technologies Used

· HTML5: Game structure and markup
· CSS3: Styling and responsive design
· Vanilla JavaScript: Game logic and AI algorithms
· Grid Layout: For the chess board

Key Algorithms

1. Move Generation: Piece-specific movement patterns
2. AI Algorithms:
   · Random selection (Easy)
   · Greedy algorithm with heuristics (Medium)
   · Minimax with evaluation function (Hard)
   · Alpha-Beta pruning with advanced evaluation (Very Hard)
3. Board Evaluation: Material counting, position scoring, mobility analysis

File Structure

```
omega-chess/
├── index.html          # Main game file (contains all code)
├── README.md           # This documentation
```

# 📄 License

This project is licensed under the MIT License

# 🙏 Acknowledgments

· Omega Chess: Created by Daniel MacDonald (1992)
· AI Algorithms: Based on classical chess AI techniques
· Icons: Unicode chess symbols and special characters
· Community: Thanks to all chess enthusiasts for inspiration

---

Enjoy the game! 🎲♟️

Remember: The beauty of chess lies not only in victory, but in the elegance of the game itself.

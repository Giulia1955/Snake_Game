# Snake_Game
🐍 Snake Game (Terminal Edition)
This is a classic Snake Game implemented in C++ that runs directly in the terminal, using POSIX terminal handling for real-time keyboard input and colored rendering with ANSI escape codes.

📦 Features
Classic snake mechanics with real-time movement.

Snake grows when eating food (@).

Game ends when colliding with walls (#) or itself.

Colored interface rendered in the terminal.

Fixed board size: 30x30.

🎮 Controls
Use the following keys to control the snake:

W – move up

A – move left

S – move down

D – move right

✅ Requirements
A Linux system or any POSIX-compliant environment (does not run natively on Windows without a terminal emulator like WSL).

A C++ compiler (e.g., g++).

A terminal that supports ANSI escape codes.

🔧 Compilation
Make sure the file Fila.h (which defines the snake structure as a linked queue) is present in the same folder. Then compile with:

bash
Copiar
Editar
g++ -o snake_game main.cpp
Replace main.cpp with the actual filename of your source code.

🚀 Running the Game
Execute the game with:

bash
Copiar
Editar
./snake_game
📂 Code Structure
kbhit() and getch(): Detect key presses without blocking the game loop.

imprimeTabuleiro(): Displays the current board state in the terminal using colors.

atualizarPosicoes(): Updates the snake's body positions based on movement.

geradorAlimento(): Randomly generates food (@) on the board.

main(): Handles game loop, collision detection, and input processing.

⚙️ Gameplay Logic
The snake is implemented as a linked queue: the head moves forward while the body follows the previous positions.

The board is redrawn each frame using system("clear") for simplicity.

When the snake eats food, a new segment is added to its tail.

Collision with the border or itself ends the game.

📸 Preview
css
Copiar
Editar
╔═══════════════════════╗
║   🐍  SNAKE GAME  🎮  ║
╚═══════════════════════╝

Use W A S D to move.
Eat the @ and avoid hitting the walls or yourself!
📌 Notes
For performance improvements, you could replace system("clear") with libraries like ncurses.

This is a great starting point for learning data structures (linked lists/queues) and terminal-based game logic.

Future improvements could include scoring, difficulty levels, or sound effects.

👨‍💻 Author
Giulia Mezaroba 
Pedro Henrique de Oliveira Ribas

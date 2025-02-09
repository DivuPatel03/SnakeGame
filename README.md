
# Snake Game in C++

## Description
This is a simple console-based Snake Game written in C++. The game features a classic snake gameplay where the player controls a snake to eat food, grow in length, and avoid collisions with the walls or itself. The game also includes a start screen, a game over screen, and simple keyboard controls.

## Features
- Console-based graphics with ASCII characters
- Start screen with instructions
- Smooth movement using keyboard inputs
- Fruit spawning and score tracking
- Game over screen with restart and quit options

## Data Structure Analysis
This game utilizes basic data structures for game logic:
- **Arrays (`tailX[]`, `tailY[]`)**: Used to store the positions of the snake's body segments. The snake's movement is managed by shifting array values.
- **Enum (`eDirection`)**: Represents the movement direction of the snake, improving code readability and preventing invalid movements.
- **Boolean Flags (`gameOver`, `gameStarted`, `showStartScreen`)**: Used for tracking the game state and controlling the flow of execution.
- **Integer Variables (`x`, `y`, `fruitX`, `fruitY`, `score`, `nTail`)**: Maintain the positions of the snake and fruit, along with the player's score and the snake's length.

## Possible Improvements
- **Linked List for Snake Body**: Instead of arrays, using a linked list would improve efficiency in handling dynamic growth of the snake's body.
- **Queue for Movement Buffering**: A queue could be used to maintain smooth movement by storing multiple inputs.

## Controls
```
W - Move Up
S - Move Down / Start the Game
A - Move Left
D - Move Right
Q - Quit the Game
R - Restart the Game (after Game Over)
```

## How to Run
1. Compile the code using a C++ compiler (such as g++ or Visual Studio).
2. Run the compiled executable in a console window.
3. Follow the on-screen instructions to start and play the game.

## Compilation Instructions
Using g++:
```sh
g++ snake_game.cpp -o snake_game.exe
```
Run the executable:
```sh
./snake_game.exe
```

## Game Logic
1. The game starts with a welcome screen displaying instructions.
2. Press 'S' to start the game, initializing the snake at the center of the screen.
3. Move the snake using W, A, S, and D keys.
4. The snake grows longer each time it eats the fruit.
5. The game ends if the snake collides with the walls or itself.
6. The final score is displayed on the Game Over screen, and the player can restart or quit.

## Dependencies
- Windows Console (for `conio.h` and `windows.h` functions)
- A C++ compiler supporting standard C++ libraries

## Known Issues
- The game currently does not support dynamic screen resizing.
- Some compilers may not support `conio.h`, requiring alternatives for input handling.

## Future Improvements
- Implement a linked list for the snake body instead of arrays.
- Add levels with increasing difficulty.
- Improve UI with better console graphics.
- Add sound effects.

## Author
Developed as part of a college project on C++ game development.

## License
This project is open-source and free to use. Modify and improve as needed!

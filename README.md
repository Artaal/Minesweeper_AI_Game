# Minesweeper AI

This is a Python project that implements a **Minesweeper game** and an AI player to solve it. The project consists of two main components:

## Minesweeper (minesweeper.py)

### Minesweeper Class

- The `Minesweeper` class represents the Minesweeper game. It allows you to initialize a game with custom dimensions and the number of mines.

- You can print the current state of the game using the `print` method, displaying the positions of mines with "X" and empty cells with spaces.

- You can check if a cell contains a mine with the `is_mine` method.

- The `nearby_mines` method returns the number of mines surrounding a given cell.

- The `won` method checks if all mines have been flagged, indicating that the player has won the game.

### Sentence Class

- The `Sentence` class represents a logical statement about the Minesweeper game. It consists of a set of board cells and a count of the number of those cells that are mines.

- The class includes methods for identifying known mines and known safe cells within the set of cells represented by the sentence.

### MinesweeperAI Class

- The `MinesweeperAI` class is responsible for playing the Minesweeper game automatically.

- It can mark cells as mines or safe, add knowledge to its knowledge base, and make safe or random moves based on its current knowledge.

## Minesweeper GUI (runner.py)

This part of the project provides a GUI for playing Minesweeper. It uses the Pygame library for the graphical interface.

- The GUI displays the Minesweeper board, allows you to click on cells to reveal them and right-click to flag them as mines.

- It provides buttons for the AI to make a move and reset the game.

- The AI agent uses the logic implemented in the `MinesweeperAI` class to make decisions on which cells to reveal or flag.

- The GUI also includes instructions on how to play Minesweeper and a play button to start the game.

## How to Play

1. Run the GUI application by executing the `runner.py` file.

2. Click on cells to reveal them and right-click to flag them as mines.

3. Use the AI Move button to let the AI make a move based on its current knowledge.

4. If you win or lose, the game will display the result.

5. You can reset the game at any time using the Reset button.

Enjoy playing Minesweeper and challenging the AI!

Please ensure you have Pygame installed to run the GUI application. You can customize the game's dimensions and the number of mines in the GUI file to adjust the difficulty level.

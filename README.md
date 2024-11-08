# Tic Tac Toe Game with AI (Depth-First Search)
This Jupyter Notebook is an implementation of a Tic Tac Toe game where the player competes against an AI opponent. The AI uses a depth-first search algorithm to select the optimal move at each turn. This project was developed as an exercise for my Artificial Intelligence Lab course at university.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [How It Works](#how-it-works)
  - [1. Game Initialization](#1-game-initialization)
  - [2. AI Move Selection (Depth-First Search)](#2-ai-move-selection-depth-first-search)
  - [3. Drawing the Game Board](#3-drawing-the-game-board)
  - [4. Saving the Game as a GIF](#4-saving-the-game-as-a-gif)
  - [5. Timing and Display](#5-timing-and-display)
  - [6. Game Flow](#6-game-flow)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Game Walkthrough](#game-walkthrough)
- [Conclusion](#conclusion)

## Introduction
This project is a Jupyter Notebook implementation of a Tic Tac Toe game where the player competes against an AI opponent. The AI uses a depth-first search (DFS) algorithm to choose the optimal move at each turn. This exercise was developed as part of my Artificial Intelligence Lab course at university.

## Features
- [ Human vs. AI gameplay using Jupyter Notebook. ]
- [AI leverages depth-first search for optimal decision-making.]
- [Graphical representation of the board using the Pillow library.]
- [Real-time tracking of elapsed time during gameplay.]
- [Saves the entire game sequence as a GIF file.]

## How It Works
### 1. Game Initialization
- [The game board is represented as a 3x3 NumPy matrix.]
- [Constants:]
  - [PLAYER = 'X': Represents the human player.]
  - [AI = 'O': Represents the AI opponent.]
  - [EMPTY = ' ': Represents empty cells on the board.]

### 2. AI Move Selection (Depth-First Search)
- [The AI uses a depth-first search (DFS) strategy to explore possible game outcomes:]
  - [If the AI finds a winning move, it returns a high score (1).]
  - [If the player's move leads to a winning state, it returns a low score (-1).]
  - [If a draw is the result, it returns a score of 0.]
- [The best_ai_move function iterates through available moves to select the one with the highest score, maximizing the AI's chances of winning.]

### 3. Drawing the Game Board
- [The Pillow library is used to create an image of the current game state:]
  - [A 3x3 grid is drawn with lines using the ImageDraw module.]
  - [The player's (X) and AI's (O) moves are displayed in different colors (red for the player and blue for the AI).]
 
### 4. Saving the Game as a GIF
- [The imageio library is used to save the sequence of board states as a GIF file.]
- [The GIF is saved in the current directory as tic_tac_toe.gif, showing the entire gameplay.]

### 5. Timing and Display
- [The time library tracks elapsed time during gameplay.]
- [The elapsed time is shown at each turn, and the total playtime is displayed at the end of the game.]

### 6. Game Flow
- [The game starts with the player making the first move, followed by the AI's turn.]
- [The game alternates turns until one of the following occurs:]
  - [The player wins.]
  - [The AI wins.]
  - [The game ends in a draw.]
- [After the game concludes, the results are displayed, and a GIF of the game is saved.]

## Requirements
The following libraries are required for this project:

- [numpy==1.24.0: For handling the game board as a matrix.]
- [pillow==9.2.0: For creating and drawing the game board images.]
- [imageio==2.35.1: For saving the game sequence as a GIF.]
- [ipython==8.26.0: For displaying images in Jupyter Notebook.]
These dependencies are specified in the requirements.txt file.

## Installation
Follow these steps to install the necessary requirements and run the project:
1. **Clone the repository** (or download the Jupyter Notebook):
```bash
git clone <your-repository-link>
cd <your-repository-folder>
```
2. **Install the required libraries** using the requirements.txt file:
```bash
pip install -r requirements.txt
```
3. **Run the Jupyter Notebook**:
```bash
jupyter notebook```
```
Open the notebook in your browser and execute the code cells to start playing.

## Usage
1. Launch the Jupyter Notebook and run the provided cells.
2. The game prompts the player to input their move as a row and column index (e.g., 1 1 for the center of the board).
3. The AI automatically makes its move based on the depth-first search algorithm.
4. The game continues until there is a winner or a draw.
5. At the end of the game, the results are displayed, and a GIF of the entire game is saved in the current directory.

## Game Walkthrough
- [Start the Game: The player is prompted to make the first move by entering the row and column indices.]
- [Display Elapsed Time: After each turn, the elapsed time is displayed in seconds.]
- [Check Game Status: The program checks if there's a winner or if the game has ended in a draw.]
- [Save the Game as a GIF: After the game concludes, a GIF of the entire gameplay sequence is saved as tic_tac_toe.gif.]

## Example Output
![Tic Tac Toe Game](tic_tac_toe.gif)

## Conclusion
This project demonstrates the use of a depth-first search algorithm to implement an AI opponent in a classic Tic Tac Toe game. The AI is designed to either win or force a draw, making it a challenging opponent. This exercise helps in understanding basic AI strategies, game trees, and the implementation of search algorithms.

Feel free to modify and extend this code for further experimentation and learning!

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
- [Human vs. AI gameplay using Jupyter Notebook.]
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

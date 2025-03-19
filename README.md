# Minesweeper AI
A Python-based Minesweeper game with an intelligent AI player.

Overview

Minesweeper is a classic puzzle game where the goal is to clear a grid without clicking on hidden mines. When a safe cell is revealed, a number appears showing how many mines are adjacent to that cell. These numbers act as clues to help decide which cells are safe to click.

This project not only recreates the Minesweeper game but also builds an AI that uses these clues. The AI uses logic to mark cells as safe or dangerous and makes smart moves to solve the board without triggering any mines.

Features

Game Setup:
Creates a board with a defined height, width, and randomly placed mines.

Clue Generation:
Each safe cell reveals a number that counts the mines in neighboring cells, providing hints to guide the next move.

AI Logic:
An AI agent gathers clues (sentences) from the revealed numbers and uses logical inference to determine which cells are safe or contain mines.

Move Selection:
The AI chooses moves based on safety: it first picks cells known to be safe, and if none are available, it selects a random move from the remaining options.

How It Works

Board Initialization:
The board is set up as a grid with hidden mines placed randomly. A cell marked with a mine is never shown until clicked by mistake.

Revealing Clues:
When a safe cell is clicked, it shows a number that indicates how many mines are in the surrounding eight cells.

AI Inference:
The AI records each move and the corresponding clue. It then builds a set of logical sentences that help deduce which neighboring cells must be mines and which are safe.

Solving the Puzzle:
By combining these clues, the AI marks cells as safe or as mines. It continues this process until all safe cells are revealed or the game is won

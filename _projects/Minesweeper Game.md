---
layout: page
title: Minesweeper Game
description: Minesweeper in Python with a logic-based assistant player.
img: /assets/img/minesweeper/minelogo.png
importance: 4
category: fun
tech_stack: [Python, Pygame, logical inference, game state modeling]
---

## Introduction

I built a playable Minesweeper game in Python with Pygame, plus a logic-based assistant that can suggest a safe move when the board gives it enough information.


![Additional Screenshot](/assets/img/minesweeper/2024-01-06%20205328.png)

## Technologies Used

- **Python**: The core programming language for the project.
- **Pygame**: Used for rendering the board and handling user input.
- **Minesweeper and AI Logic**: Custom Python classes to handle the game logic and AI decision-making.

## Game Features

- **Standard Minesweeper Gameplay**: Users can click to reveal cells and right-click to place flags on cells where they suspect mines are located.
- **AI Integration**: At any point during the game, players can invoke an AI agent to make a safe move or a random move if no obvious safe moves are available.
- **Customizable Difficulty**: The game's grid size and the number of mines can be adjusted to change the difficulty level.
- **Graphical Interface**: The board shows mines, flags, and nearby mine counts clearly.

## Development Process

1. **Setting Up Pygame**: The first step involved setting up Pygame and creating a basic window where the game would be played.
2. **Designing the Game Board**: I defined the game board using a grid system. Each cell in the grid could either contain a mine or a number indicating the count of adjacent mines.
3. **Implementing Game Logic**: The core logic of Minesweeper, including mine placement and game rules (revealing cells, game win/loss conditions), was implemented.
4. **AI Agent Development**: I developed an AI agent using logical reasoning. The AI uses knowledge about safe and mined cells to make informed decisions.
5. **User Interface Design**: I added a user-friendly interface, including buttons for user interactions like resetting the game or asking the AI for help.
6. **Testing and Refinement**: The final stage involved thorough testing and refining the game's mechanics and AI's decision-making process.

## Challenges and Learnings

- **AI Implementation**: Developing an AI agent that makes decisions based on the current state of the game was challenging and required a good understanding of logical deduction and Minesweeper's rules.
- **Pygame Mechanics**: I used Pygame for rendering, clicks, resets, and board updates.

## Notes

The interesting part was translating Minesweeper rules into a small knowledge base: known safe cells, known mines, and sentences about unresolved cells.

## Screenshots

![Minesweeper Game Screenshot](/assets/img/minesweeper/Screenshot%202024-01-06%20205523.png)
![Additional Screenshot](/assets/img/minesweeper/010602.png)


## Check Out the Code

The implementation, including the assistant player, is available on GitHub.

[View the Minesweeper Project on GitHub](https://github.com/Michael-xliu/minesweeper)

The repository includes the game logic, assistant logic, and Pygame interface.



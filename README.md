## 2-Player Memory Game (Jack | Nand2Tetris)

## Overview

This project is a **2-player Memory Card Game** built using the **Jack programming language** in the Nand2Tetris environment.

Two players take turns flipping cards to find matching pairs.

* If the cards match → player earns a point
* If not → cards flip back and turn switches

The game continues until all pairs are matched, and the player with the highest score wins.

---

## Features

* Two-player gameplay
* Turn-based system
* Card matching logic
* Separate scoreboard for Player 1 and Player 2
* Modular design using multiple Jack classes
* Runs on Nand2Tetris VM Emulator

---

## Project Structure

```
memory_game/
│
├── memory_game_jack/   # Jack Source Code
│   ├── Main.jack
│   ├── Game.jack
│   ├── Board.jack
│   ├── Card.jack
│   ├── UI.jack
│   └── Input.jack
│
├── memory_game_VM/     # Compiled VM Code
│   ├── Main.vm
│   ├── Game.vm
│   ├── Board.vm
│   ├── Card.vm
│   ├── UI.vm
│   └── Input.vm
│
└── README.md
```

---

##  How to Run

### Method 1: Run Using VM Files (Recommended)

1. Open **Nand2Tetris VM Emulator**
2. Click **Load Program**
3. Select folder:

   ```
   memory_game_VM
   ```
4. Click **Run**
5. The game starts from `Main.vm`

---

### Method 2: Compile from Jack Files

1. Open **Jack Compiler**
2. Load folder:

   ```
   memory_game_jack
   ```
3. Compile all `.jack` files
4. This generates `.vm` files
5. Open VM Emulator → Load → Run

---

## How to Play

1. The board displays hidden cards
2. Player 1 starts the game
3. Select two card positions
4. Cards flip and reveal values

   * If matched → player gets 1 point
   * If not → cards flip back
5. Turn switches to Player 2
6. Repeat until all pairs are matched

---

## Game End & Winner

* Game ends when all cards are matched
* Player with highest score wins 

---

## Scoring System

* Match → +1 point
* No match → Turn changes
* Highest score → Winner

---

##  Modules Explanation

###  Main.jack

* Entry point of the program
* Starts the game

###  Game.jack

* Controls game flow
* Manages turns between players
* Updates scores and checks game end

###  Board.jack

* Manages the grid of cards
* Handles flipping and matching logic

###  Card.jack

* Represents each card
* Stores:

  * Card ID
  * Flip state
  * Match status

###  UI.jack

* Displays board and scores
* Updates screen after each move

###  Input.jack

* Takes player input
* Sends selected positions to game logic

---

##  Game Flow

Start → Initialize Board → Player Turn → Flip Cards →
Check Match → Update Score → Switch Turn → Repeat → End Game

---

##  Requirements

* Nand2Tetris VM Emulator
* Jack Compiler

---

##  Future Enhancements

* GUI-based interface
* Difficulty levels (larger grid)
* Timer-based scoring
* Sound effects
* Single-player mode with AI

---





# Pup Rescue: Lawn Block

A GUI puzzle game inspired by the classic *Rush Hour* game, developed with Python and Pygame.

Players must help the puppy escape the grass maze by moving obstacles strategically within a 6×6 grid.

---

# 🎮 Game Overview

In this game:

* The red vehicle is replaced by a puppy 🐶
* Other vehicles become lawn blocks 🌿
* Players can only move objects along their original direction
* The goal is to clear a path for the puppy to reach the exit

The project extends the traditional Rush Hour puzzle with:

* GUI interaction
* Multiple challenge modes
* Hint system
* Undo system
* Remove power-up
* Save & Load system
* Sound effects and animations

---

# ✨ Features

## Core Gameplay

* 6×6 puzzle board
* Collision detection
* Boundary checking
* Win condition detection
* Smooth movement animation

---

## GUI System

* Main menu
* Level selection screen
* In-game HUD
* Pause panel
* Win / Fail panels
* Hover effects and button feedback

---

## Challenge Modes

### Normal Mode

* No constraints
* Free exploration

### Limited Time Mode

* Countdown timer
* Fail when time runs out

### Limited Step Mode

* Limited number of moves
* Strategic gameplay

---

## Advanced Features

### Undo System

* Restore previous game state
* Supports multiple undo operations

### Hint System

* Suggests useful moves when the player is stuck
* BFS-based solving logic

### Remove Power-up

* Removes one blocking obstacle temporarily
* Supports undo recovery

### Save & Load

* Save:

  * current level
  * timer
  * steps
  * stars
  * unlocked levels
  * challenge progress
* Automatically restore progress after restarting the game

---

## Audio System

Includes:

* Background music
* Move sound
* Button click sound
* Error sound
* Win / fail sound effects

---

# 🧠 Technical Highlights

## Object-Oriented Design

The project uses modular architecture:

```text
Game
├── UI
├── GameState
├── AudioManager
├── SaveManager
└── Vehicle / Board Models
```

---

## State Management

The game stores:

* vehicle positions
* remaining steps
* timer
* remove counts
* unlock progress

This ensures reliable gameplay and save/load consistency.

---

## BFS Hint Algorithm

The hint system uses Breadth-First Search (BFS):

```text
Current State
↓
Generate Next States
↓
Check Valid Moves
↓
Search for Solution
↓
Return Recommended Move
```

---

## Animation & Feedback

The game improves user experience with:

* smooth movement interpolation
* invalid move shake animation
* hover feedback
* audio response

---

# 🛠️ Technologies Used

* Python 3
* Pygame
* JSON
* Object-Oriented Programming
* BFS Algorithm
* Git & GitHub Collaboration Workflow

---

# 📂 Project Structure

```text
RushHourPy/
├── assets/
│   ├── audio/
│   ├── images/
│   └── fonts/
│
├── game/
│   ├── game.py
│   ├── state.py
│   ├── vehicle.py
│   ├── constants.py
│   └── save_manager.py
│
├── ui/
│   ├── button.py
│   ├── panels.py
│   └── hud.py
│
├── solver/
│   └── bfs_solver.py
│
├── main.py
├── requirements.txt
└── README.md
```

---

# 🚀 Installation

## 1. Clone the Repository

```bash
git clone https://github.com/OceanHope315/RushHourPy.git
```

---

## 2. Enter the Project Directory

```bash
cd RushHourPy
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Run the Game

```bash
python main.py
```

---

# 🎯 Controls

| Action          | Control               |
| --------------- | --------------------- |
| Select Vehicle  | Mouse Click           |
| Move Vehicle    | Mouse Drag / Keyboard |
| Undo            | Undo Button           |
| Hint            | Hint Button           |
| Remove Obstacle | Remove Button         |
| Pause           | Pause Button          |

---

# 👥 Team Collaboration

This project was developed collaboratively using:

* Lark for task assignment and discussion
* GitHub for version control
* Pull Request workflow for code review and merging

Team members worked on:

* UI system
* game logic
* audio system
* advanced features
* animations and effects

---

# 📈 Future Work

Planned improvements include:

* More puzzle levels
* Smarter AI hint system
* Custom level editor
* Online leaderboard
* Better animations
* Mobile adaptation

---

# 📸 Screenshots

## Main Menu

(Add screenshot here)

## Gameplay

(Add screenshot here)

## Challenge Modes

(Add screenshot here)

## Win Panel

(Add screenshot here)

---

# 🙌 Acknowledgements

Inspired by the classic *Rush Hour* puzzle game.

Developed as a university GUI game project using Python and Pygame.

---

# 📄 License

This project is for educational purposes only.

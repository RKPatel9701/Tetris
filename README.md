# Console Tetris (C++)

A classic **Tetris** game built in **C++** for the Windows console. The game features all seven classic tetrominoes, smooth keyboard controls, colorful blocks, real-time scoring, and flicker-free console rendering.

---

## Overview

This project is a console-based implementation of the classic **Tetris** game developed in **C++**. It uses Windows Console APIs for rendering and keyboard input, providing an interactive gaming experience entirely within the terminal.

The project demonstrates fundamental programming concepts such as arrays, object-oriented programming (OOP), collision detection, game loops, real-time input handling, and basic game development.

---

## Features

- All 7 classic tetrominoes (I, O, T, S, Z, J, L)
- Distinct colors for each tetromino
- Arrow Keys and WASD controls
- Hard drop using the Spacebar
- Piece rotation
- Automatic line clearing
- Real-time score calculation
- High score tracking during the application's runtime
- Flicker-free console rendering
- Restart after Game Over
- Exit option after Game Over

---

## Requirements

- Windows Operating System
- C++ Compiler
  - MSVC (Visual Studio)
  - MinGW (g++)
- Windows-specific libraries:
  - `windows.h`
  - `conio.h`

---

## Build and Run

### Using MinGW (g++)

```bash
g++ tetris.cpp -o tetris.exe -static
./tetris.exe
```

### Using MSVC

Open the **Developer Command Prompt for Visual Studio** and run:

```bash
cl tetris.cpp
tetris.exe
```

---

## Controls

| Key | Action |
|------|--------|
| ← / A | Move Left |
| → / D | Move Right |
| ↓ / S | Soft Drop |
| ↑ / W | Rotate Piece |
| Spacebar | Hard Drop |
| R | Restart (after Game Over) |
| X | Exit (after Game Over) |

---

## How It Works

The game uses a fixed-size 2D grid to represent the playing field. Each tetromino is stored as a matrix and rendered onto the board using Windows Console APIs.

The implementation includes:

- Random tetromino generation
- Collision detection
- Piece movement and rotation
- Automatic gravity
- Line detection and clearing
- Score calculation
- High-score tracking within the application session
- Efficient in-place rendering using `SetConsoleCursorPosition()` to eliminate screen flickering

---

## Project Structure

```text
Console-Tetris/
│
├── tetris.cpp
└── README.md
```

---

## Technologies Used

- C++
- Object-Oriented Programming (OOP)
- Windows Console API
- Standard Template Library (STL)

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Object-Oriented Programming (OOP)
- Real-time game loop implementation
- Collision detection algorithms
- Matrix-based game representation
- Console graphics programming
- Keyboard input handling
- Game logic and scoring systems
- Efficient rendering techniques

---

## Future Improvements

- Next piece preview
- Hold piece functionality
- Increasing difficulty levels
- Persistent high-score file storage
- Pause and resume feature
- Sound effects and background music

---

## Author

**Rashi Patel**

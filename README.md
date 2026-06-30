# Console Tetris (C++)

A classic Tetris game built in C++ for the Windows console, featuring colored 
blocks, smooth controls, and persistent high score tracking within a session.

## Features
- Full set of 7 tetrominoes (I, O, T, S, Z, J, L) with distinct colors
- Arrow key or WASD controls
- Hard drop with spacebar
- Line clearing and scoring
- High score tracking across multiple game sessions (Restart without closing)
- In-place console rendering (no flicker)

## Requirements
- Windows OS (uses `<windows.h>` and `<conio.h>`)
- A C++ compiler (MSVC, MinGW, or similar)

## Build

### Using g++ (MinGW)
```bash
g++ tetris.cpp -o tetris.exe -static
./tetris.exe
```

### Using MSVC (Developer Command Prompt)
```bash
cl tetris.cpp
tetris.exe
```

## Controls
| Key            | Action          |
|----------------|-----------------|
| ← / A          | Move left       |
| → / D          | Move right      |
| ↓ / S          | Soft drop       |
| ↑ / W          | Rotate          |
| Spacebar       | Hard drop       |
| R (after game over) | Restart    |
| X (after game over) | Exit       |

## How It Works
The game grid is a fixed-size 2D character array. Each tetromino is represented 
as a small matrix of IDs (1–7), which is overlaid onto the grid each frame and 
rendered using `SetConsoleCursorPosition` for flicker-free updates. Collision 
detection (`canMove`) checks boundaries and occupied cells before allowing 
movement or rotation. Completed rows are detected and cleared in `clearLines`.

## License
MIT License — feel free to use, modify, and distribute.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to 
discuss what you'd like to change.

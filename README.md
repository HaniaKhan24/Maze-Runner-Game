# Arcane Maze Generator

A C++ game project that procedurally generates mazes using data structures and algorithms, featuring an interactive player experience with hint system and timed gameplay.

## Project Overview

This is a Data Structures and Algorithms (DSA) project that implements maze generation and pathfinding algorithms. The game creates random mazes using graph-based techniques and provides an interactive interface for players to navigate through the generated maze.

## Features

- Procedural maze generation using depth-first search and backtracking
- Interactive player movement and collision detection
- Real-time timer for timed challenges
- Hint system that displays a path to the treasure/exit
- Audio and visual assets for enhanced user experience
- Start page, win page, and lose page screens
- Customizable maze dimensions and cell sizes

## Project Structure

```
Group_02_DSA_Project/
├── main.cpp                  # Main game loop and window management
├── include/
│   ├── Graph.h              # Maze structure and generation
│   ├── Cell.h               # Individual maze cell representation
│   ├── Player.h             # Player movement and interaction
│   ├── Stack.h              # Stack data structure for backtracking
│   └── Queue.h              # Queue data structure
├── src/
│   ├── Graph.cpp            # Graph implementation
│   ├── Cell.cpp             # Cell implementation
│   ├── Player.cpp           # Player implementation
│   ├── Stack.cpp            # Stack implementation
│   └── Queue.cpp            # Queue implementation
├── assets/
│   └── sounds/              # Audio files for game
├── bin/                      # Compiled binaries
│   ├── Debug/
│   └── Release/
├── obj/                      # Object files
│   ├── Debug/
│   └── Release/
└── Group_02_DSA_Project.cbp # Code::Blocks project file
```

## Technologies Used

- **Language**: C++
- **Graphics Library**: SFML (Simple and Fast Multimedia Library)
- **Audio Library**: SFML Audio
- **Build System**: Code::Blocks
- **Data Structures**: Stack, Queue, Graph (Adjacency Matrix)
- **Algorithms**: Depth-First Search (DFS) with backtracking

## Core Data Structures

- **Graph**: Represents the maze using an adjacency matrix
- **Stack**: Used for backtracking during maze generation
- **Queue**: Utility data structure for the project
- **Cell**: Individual units of the maze grid

## Building and Running

### Prerequisites
- C++11 or later
- SFML library
- Code::Blocks IDE (or any C++ compiler)

### Compilation
1. Open `Group_02_DSA_Project.cbp` in Code::Blocks
2. Build the project using Build menu
3. Run the executable from the bin/Debug or bin/Release folder

### Required Assets
The project requires the following asset files:
- `arial.ttf` - Font file for UI text
- `assets/start-page.png` - Start screen image
- `assets/win-page.png` - Win screen image
- `assets/lose-page.png` - Lose screen image
- `assets/sounds/` - Audio files for game effects

## Gameplay

1. The game starts with a randomly generated maze (15 rows × 20 columns)
2. Player starts at the bottom-right corner
3. Navigate through the maze using arrow keys or WASD
4. Reach the treasure/exit to win
5. Use the Hint button to display the path to the exit
6. Complete the maze before time runs out
7. Timer displays elapsed time during gameplay

## Algorithm Details

### Maze Generation
The maze is generated using a depth-first search algorithm with backtracking:
1. Start from a random cell
2. Mark current cell as visited
3. Choose a random unvisited neighbor
4. Remove walls between cells
5. Recursively process the neighbor
6. Backtrack when no unvisited neighbors are available

## Team

Group 02 - DSA Project

## License

This project is part of an academic assignment.

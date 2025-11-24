# Project(EXE) - Maze Game

---

## English Explanation

### Project Overview
This project is a console-based **Maze Game** written in **x86 Assembly (TASM)**. The game allows a player to navigate through a maze while avoiding enemies and reaching the winning point.

### Features
- Player movement using arrow keys.
- Two enemies moving randomly.
- Collision detection with walls and enemies.
- Winning and losing conditions.
- Color-coded display for the player, enemies, start, and end points.
- Simple user interface with instructions.

### Code Breakdown

#### Macros
- **SetResolution**: Scrolls specific rows and columns with a given attribute.
- **copy**: Copies the current position (row/column) into another variable.
- **print**: Prints a string using DOS interrupt 21h.
- **write**: Writes a character at the current cursor position with attributes.
- **setCursor**: Moves the cursor to a specific row and column.

#### Data Segment
- Variables store player and enemy positions, old positions, and strings for messages like welcome, winning, and losing.
- Example:  
```asm
row1 db 23      ; Player's row
col1 db 37      ; Player's column

# Maze Pathfinding Visualizer

Maze pathfinding visualizer using Python's curses module. The program uses BFS to find the shortest path in a maze from a start position (O) to an end position (X).

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/maze-pathfinding-visualizer.git

   cd maze-pathfinding-visualizer

2. Create and activate a virtual environment (optional but recommended):
   ```
   python -m venv venv

   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install packages:
   ```
   pip install -r requirements.txt


##Code Overview

###maze
The maze is a 2D list representing the maze structure. # represents walls, spaces represent open paths, O is the start, and X is the end.

###print_maze(maze, stdscr, path=[])
This function prints the maze to the screen, with an optional path highlighted in red.

###find_start(maze, start)
This function finds the starting position in the maze.

###find_path(maze, stdscr)
This function uses BFS to find the shortest path from the start to the end. It updates the screen to visualize the search process.

###find_neighbors(maze, row, col)
This function returns the valid neighbors (up, down, left, right) of a given position in the maze.

###main(stdscr)
This is the main function that initializes color pairs and starts the pathfinding visualization.

###wrapper(main)
This function is provided by the curses module to handle the initialization and teardown of the terminal window.



Example:

# X # # # # # # #
# X             #
# X # #   # #   #
# X #       #   #
# X #   #   #   #
# X #   #   #   #
# X #   #   # # #
# X X X X X X X #
# # # # # # # X #

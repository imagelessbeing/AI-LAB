🧩 8-Puzzle Solver using DFS and BFS (Python)

This project implements a solution to the classic 8-puzzle problem using Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms in Python.

The 8-puzzle consists of a 3x3 grid with 8 numbered tiles and a single blank space (represented by 0). The objective is to rearrange the tiles to match a predefined goal configuration using legal moves.
📌 Problem Statement

Given an initial state of the puzzle, determine a sequence of valid moves (up, down, left, right) to reach the goal state by sliding the blank tile (0) into adjacent positions.

This implementation verifies whether the goal is reachable and demonstrates the path to the solution using both DFS and BFS.
✨ Features

    Solves the 8-puzzle using:

        ✅ Depth-First Search (DFS)

        ✅ Breadth-First Search (BFS)

    Represents puzzle state using nested Python lists (List[List[int]])

    Dynamically generates valid moves

    Tracks visited states to avoid redundant exploration

    Clean and readable codebase

🛠️ Implementation Details
🐍 Programming Language

    Python 3

📚 Data Structures Used

    list of list: To represent the puzzle grid

    set or dict: To track visited states

    stack: For DFS (can use a Python list)

    queue: For BFS (from collections.deque)

🔧 Key Functions
Function Name	Description
print_state(state)	Prints the current puzzle state in a readable format
is_goal(state)	Checks if a given state matches the goal state
get_blank_pos(state)	Returns the coordinates of the blank tile (0)
generate_children(state)	Generates all valid child states by moving the blank tile
dfs(start_state)	Solves the puzzle using Depth-First Search
bfs(start_state)	Solves the puzzle using Breadth-First Search
state_to_tuple(state)	Converts state to a hashable tuple for visited tracking

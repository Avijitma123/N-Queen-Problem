N-Queens Problem Solver
Overview
This C++ program provides a solution to the classic N-Queens problem, where N queens must be placed on an NxN chessboard without attacking each other. The program utilizes a Breadth-First Search (BFS) approach to explore possible configurations and identify solutions.

Author
Avijit Dey
Roll: 2022SMCS006

Code Structure
Classes
Node: Represents the state of the chessboard. The putQueen, display, and other methods assist in handling the state information.
Queues
q: Stores successor states during the search.
gq: Stores goal states (solutions).
nonAt: Stores non-attacking states.
Functions
isSafe(Node node, int x, int y): Checks if placing a queen at a specific position is safe.
isGoal(Node node): Determines if a state is a goal state (solution).
isRepeated(Node node): Checks if a state is repeated in the search.
findSuccessor(Node node): Finds successor states by placing queens in safe positions.
TreeSearch(): Conducts the BFS to explore states and find solutions.
Execution
The main function initiates the BFS by calling TreeSearch(). The program outputs the total number of solutions, the number of non-attacking solutions, and displays each solution's chessboard configuration.

How to Use
Compile the code using a C++ compiler.
Run the executable.
The program will output the number of solutions, the number of non-attacking solutions, and display each solution's chessboard configuration.
Example Output
bash
Copy code
Number of solutions: 92
Number of non-attacking solutions: 12

Solution 1
1 0 0 0 0 0 0 0 
0 0 0 0 0 0 1 0 
0 1 0 0 0 0 0 0 
0 0 0 0 1 0 0 0 
0 0 0 0 0 0 0 1 
0 0 1 0 0 0 0 0 
0 0 0 0 0 1 0 0 
0 0 0 1 0 0 0 0 
====================

...
Contributions
Contributions and improvements to the code are welcome. Feel free to fork the repository, make changes, and submit pull requests.


Counting Islands
This project provides a solution to count the number of islands in a given map, where an island is defined as a connected region of 1's (land) surrounded by 0's (water) in an MxN matrix.

Approach
The solution uses a depth-first search (DFS) algorithm to traverse the matrix and identify connected regions of 1's. The algorithm iterates over each cell in the matrix, and when it encounters a cell with a value of 1, it performs a DFS to mark all connected 1's as visited. The number of times the DFS is performed corresponds to the number of islands in the map.

Usage
To run the solution, simply execute the count_islands function in the island_counter.py script, passing in a 2D list representing the map. For example:

map = [  [0, 1, 0],
  [0, 0, 0],
  [1, 1, 1]
]

count = count_islands(map)
print(count)  # output: 1

Test Cases
The solution has been tested with the following input maps:

3x3 map with 2 islands:

[
  [0, 1, 0],
  [0, 1, 0],
  [0, 0, 1]
]


3x4 map with 3 islands:

[
  [0, 0, 1, 0],
  [0, 1, 0, 1],
  [0, 1, 1, 1]
]


3x4 map with 2 islands:


[
  [0, 0, 1, 0],
  [0, 1, 1, 0],
  [0, 1, 0, 1]
]


Dependencies
The solution has been implemented in Python 3 and does not have any external dependencies.
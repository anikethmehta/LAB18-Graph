### ***Date*** : 23 November
### ***Title*** : LAB18-Graph
### ***Aim*** : Graph Data Structure
### ***Algorithm*** :

Adjacency Matrix to Adjacency List:

Initialize an empty adjacency list for each vertex.

For each row in the adjacency matrix:
Create an empty list to represent the neighbors of the current vertex.

For each entry in the row:

If the entry is non-zero (indicating an edge):

Add the corresponding column index to the list of neighbors for that vertex.

Repeat steps 2-3 for each row in the matrix.

The resulting lists represent the adjacency list for each vertex.

Adjacency List to Adjacency Matrix:

Initialize an empty adjacency matrix with all entries set to zero.

For each vertex in the adjacency list:

For each neighbor in the list:

Set the corresponding entry in the adjacency matrix to 1.

Repeat step 2 for each vertex in the adjacency list.

The resulting matrix represents the adjacency matrix for the graph.

### ***Explanation*** :
1. Graph Class:
   
A Graph is like a map that shows connections between different locations (vertices/nodes).
It uses an adjacency matrix to represent which locations are directly connected.

2. Functions in the Graph Class:
   
2.1 addEdge Function:
Adds a connection between two locations (vertices).
If there's an edge between vertex A and vertex B, it's also added between B and A (for an undirected graph).

2.2 BFS Function:
Uses Breadth-First Search to visit and print each location in a systematic order.
Starts from a specified location (vertex) and explores its neighbors before moving on to the next level.

2.3 DFS Function:
Uses Depth-First Search to visit and print each location.
Starts from a location and goes as deep as possible before backtracking.

2.4 convertToAdjacencyList Function:
Converts the adjacency matrix to an adjacency list.
An adjacency list is like a list of friends for each person, indicating who they are directly connected to.

2.5 convertToAdjacencyMatrix Function:
Converts the adjacency list back to an adjacency matrix.
This is like turning the list of friends into a matrix that shows who is friends with whom.

3. Example in the main Function:
Creates a graph with 6 locations.
Adds connections between these locations.
Shows BFS and DFS traversal starting from location 0.
Converts between adjacency matrix and adjacency list, then prints them.

4. Printing:
cout is used to print information to the console.
The printed information includes traversal results and the converted representations of the graph.

5. Overall:
The code helps you create, explore, and represent a graph.
It shows different ways of looking at the connections in the graph, making it useful for various algorithms and analyses.

### ***Output Screenshot*** :

Code:

Output:

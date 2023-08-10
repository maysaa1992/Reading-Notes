# Graphs
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.some common terminology used 
 ## when working with Graphs:

1-Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.

2-Edge - An edge is a connection between two nodes.


3-Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.


4-Degree - The degree of a vertex is the number of edges connected to that vertex.


## Directed vs Undirected
* Undirected Graphs
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

For example, in the graph below, Node C is connected to Node A, Node E and Node B. There are no “directions” given to point to specific vertices. The connection is bi-directional.

* Directed Graphs (Digraph)
A Directed Graph also called a Digraph is a graph where every edge is directed.

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.



## Connected
A connected graph is graph that has all of vertices/nodes have at least one edge.

## Disconnected
A disconnected graph is a graph where some vertices may not have edges.

## Acyclic vs Cyclic
In addition to undirected and directed graphs, we also have acyclic and cyclic graphs.

## Traversals
You will be required to traverse through a graph. The traversals itself are like those of trees. Below is a breakdown of how you would traverse a graph.

Breadth First
In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. The breadth first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Traversing a graph that has cycles will result in an infinite loop….this is bad. To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.

As a refresher of what breadth first actually means here it is: Breadth first traversal is when you visit all the nodes that are closest to the root as possible. From there you traverse outwards, level by level, until you have visited all the vertices/nodes.

Here is what the algorithm breadth first traversal looks like:

1- Enqueue the declared start node into the Queue.


2- Create a loop that will run while the node still has nodes present.


3-Dequeue the first node from the queue


4-if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.  
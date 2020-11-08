---
layout: post
title:      "Introduction to Greedy Algorithms"
date:       2020-11-08 20:17:22 +0000
permalink:  introduction_to_greedy_algorithms
---


A greedy algorithm is not a morally corrupt algorithm. Actually, greedy algorithms are algorithms that take the best results for each individual step of the problem, rather than looking at the problem as a whole. Greedy Algorithms do not always find the optimal solution, but is a good option when considering possible strategies in solving problems. Two examples of greedy algorithms are Dijkstra's Algorithm and Huffman Encoding. These two examples are commonly used and are have some very useful applications.

Acording to brilliant.org, greedy algorithm can be used in a problem if the two properties are true:

"**Greedy choice property:** A global (overall) optimal solution can be reached by choosing the optimal choice at each step.

**Optimal substructure:** A problem has an optimal substructure if an optimal solution to the entire problem contains the optimal solutions to the sub-problems."

Dijkstra's Algorithm is used to find the shortest path in a graph. It is commonly used for finding distances between physical locations and in routing protocols. In each step, it will find the next node with the shortest distance. This will not always find the shortest solution because it does not look at the graph as a whole. 

Here is psudocode for Dijkstra;s Algorithm, taken from [here](http://www.gitta.info/Accessibiliti/en/html/Dijkstra_learningObject1.html).
```
function Dijkstra(Graph, source):
2:	for each vertex v in Graph:	// Initialization
3:	dist[v] := infinity	// initial distance from source to vertex v is set to infinite
4:	previous[v] := undefined	// Previous node in optimal path from source
5:	dist[source] := 0	// Distance from source to source
6:	Q := the set of all nodes in Graph	// all nodes in the graph are unoptimized - thus are in Q
7:	while Q is not empty:	// main loop
8:	u := node in Q with smallest dist[ ]
9:	remove u from Q
10:	for each neighbor v of u:	// where v has not yet been removed from Q.
11:	alt := dist[u] + dist_between(u, v)
12:	if alt < dist[v]	// Relax (u,v)
13:	dist[v] := alt
14:	previous[v] := u
15:	return previous[ ]
```

There are many variants of Dijkstra's Algorithm. Many times, a shortest path tree, which finds the shortest paths of a given node to every other node. 

The Huffman Encoding algorithm is used to remove ambiguity in encoding characters. According to [Geeks for Geeks](https://www.geeksforgeeks.org/huffman-coding-greedy-algo-3/), "Prefix Codes, means the codes (bit sequences) are assigned in such a way that the code assigned to one character is not the prefix of code assigned to any other character." This ensures there is no confusion in decoding the characters. There are two steps to this algorithm: first to build a Huffman Tree from input characters, and seccond to traverse the Huffman Tree and assign codes to characters.

There are just two examples of greedy algorithms. Programmers use create their own solutions using greedy algorithms all the time. Other examples of greedy algorithms include Activiy Selection Problem, Egyption Fraction, Job Sequencing Problem, Huffman Decoding, Water Connection Problem, Policeman Catch Thieves, Minimum Swaps for Bracket Balancing, and more. There are many websites that give practice problems to solve, including Brilliant, HackerRank, TopCode, and GeekForGeeks. There are also many websites that provide more learning resources. 

Sources:

https://www.algorithmhalloffame.org/algorithms/dijkstras-algorithm/#:~:text=The%20algorithm%20exists%20in%20many,producing%20a%20shortest%2Dpath%20tree.

https://brilliant.org/wiki/greedy-algorithm/#:~:text=A%20greedy%20algorithm%20is%20a,to%20solve%20the%20entire%20problem.

https://www.geeksforgeeks.org/dijkstras-shortest-path-algorithm-greedy-algo-7/

https://www.geeksforgeeks.org/huffman-coding-greedy-algo-3/

http://www.gitta.info/Accessibiliti/en/html/Dijkstra_learningObject1.html

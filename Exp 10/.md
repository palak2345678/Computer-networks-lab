# EXPERIMENT 10

Implementation of Distance Vector Routing Algorithm

## THEORY
The **Distance Vector Routing** algorithm is a dynamic routing protocol where each router maintains a routing table indexing the least-cost path to every other node in the network. Each router periodically shares its routing table vector (distances to all known destinations) with its immediate neighboring routers. 

Using the **Bellman-Ford equation**, routers iteratively update their routing tables when a shorter path via a neighbor is discovered:
$$D_x(y) = \min_v \{ c(x,v) + D_v(y) \}$$

## TERMINAL SESSION
```
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ vim distance_vector_1221.c
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ gcc distance_vector_1221.c -o distance_vector
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ ./distance_vector
Enter the number of routers: 3
Enter the cost matrix (use 999 for infinity/no direct link):
0 2 5
2 0 1
5 1 0

\nRouter info for router: 1
Dest Node	Next Hop	Distance
1		1		0
2		2		2
3		2		3

Router info for router: 2
Dest Node	Next Hop	Distance
1		1		2
2		2		0
3		3		1

Router info for router: 3
Dest Node	Next Hop	Distance
1		2		3
2		2		1
3		3		0
```

## CONCLUSION
The Distance Vector Routing algorithm was successfully implemented in C. Using iterative neighbor state sharing and cost calculations, each router successfully constructed its optimal routing table with least-cost paths and corresponding next-hop destinations.

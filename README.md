# Rumor Algorithm

Rumor Algorithm is a heuristic algorithm for solving TSP problems (both directed and undirected graphs).

It is based on the idea that, experiences of humans in a population effect the decisions of others. Conveying the experiences to the others (rumor) basically makes new decisions positively or negatively biased. Influence factor of these experiences is not linear and often experiences are evaluated with respect to the average, the best and the worst outcomes of these experiences. 

For the min weighted TSP problem setting, experiences are the routes taken (arc sequence) and their associated total weights (distance, cost, time etc.), that is the outcome. Collection of rumors about these routes (sequence of nodes that form a hamiltonian cycle) generates influence on the next group of humans and effect their decions in route selection. Greedy algorithms selects the minimum weighted arc at each node and this often leads to very suboptimal solutions (unless, luckily finds a good solution by chance). Algorithms such as Ant Colony Optimiztion (ACO) and Artificial Bee Colony (ABC) mimic the behavior of ant and bee colonies by using passing experiences and collective knowladge gained to the colony for making better and better decisions in time. Rumor algorithm,       

In Rumor Algorithm, these groups of people are represented as populations in human waves. A human wave is a collection of humans seeking for a feasible tsp route.

At ititial wave (wave 0) in agorithm; a population of humans is sent to the tsp graph to find tsp routes totally randomly. That is, a number of feasible routes are generated randomly. It is technically possible to have routes having the same node seqeunce. But,it is ensured that the routes sequences are unique (that is every human follows a different route, although they may have common arcs in their routes). Population size at the initial wave as well as population growth or decrease rates are parameters in the algorithm. Results of the routes of initial wave of humans construct the initial influences about the graph and its arcs.   
Very small initial population size results in less exploration of the graph, however larger the population     

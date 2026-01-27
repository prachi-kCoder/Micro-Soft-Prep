# CHEAPEST FLIGHTS WITHIN K-STOPS 
- BELIVE IT simple level-wise BFS by stops is the best way to solve this problem !, no 2d array necessary , best optimal
- SIMPLE STOP WISE LEVEL BFS allows us to explore all possible paths with k stops limit & relaxing the cost[u]/ dist[u]
- DO NO FORGET : `next_dist and dist array` separate to keep prev level data is used for next level, no currlevel data to be used ,
- `cost < dist[u]` : Allows best path to explore , from prev level elmination Stale data ! on only exploring least cost path to u further !
- Do it here : https://leetcode.com/problems/cheapest-flights-within-k-stops/submissions/1842987200/

# Redundant connectioon2 :
- https://leetcode.com/problems/redundant-connection-ii/
- Best way to know when DSU fails specifically in directed graphs how to handle it
  
# shortest path to get all keys :
- Again all keys by level wise bfs + bitmask dp , TC = O( n X x X (1<<k)) , SC = O(n x n x (1<<K))
- Do :https://leetcode.com/problems/shortest-path-to-get-all-keys/submissions/1882601996/
  
# Course-Schedule-II
- Donot forget to check for cycle after getting topo order of courses .
- KEEP IN MIND : Kahn's algo (a,b) where a says go do b first then indeg of b in inc and b->a graph formed , but in DFS we do the rev a->b and do a post order dfs ie for a we do and visit all its nbr
- TC : O(V+E) ie because for all V nodes all e edges are checked no matter we get another v node or not ? , SC = O(V+E) -> adj list 
- DO : https://leetcode.com/problems/course-schedule-ii/

# SHORTEST PATH VISITING ALL NODE :
- BIMASK + GRAPH: DO HERHE :https://leetcode.com/problems/shortest-path-visiting-all-nodes/submissions/1882060876/
- tc = n * (2^N) , SC = O(N*(2^N) )   {as visiting the pair of node , bitmask is necessary to avoid infinitel loop }
  
# Parallel courses-III
- DP + Topological Order , TC = O(V + E) , SC = O(V + E)
- https://leetcode.com/problems/parallel-courses-iii/submissions/1876409560/

# ROTTEN ORANGES : 
- DO : https://www.geeksforgeeks.org/problems/rotten-oranges2536/1
- Keep in mind level-wise BFS is fastest approach O(N X M) & SC = O(1) no extra space , we can directly use the matrix given in problem ! 

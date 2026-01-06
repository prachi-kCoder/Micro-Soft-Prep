# CHEAPEST FLIGHTS WITHIN K-STOPS 
- BELIVE IT simple level-wise BFS by stops is the best way to solve this problem !, no 2d array necessary , best optimal
- Do it here : https://leetcode.com/problems/cheapest-flights-within-k-stops/submissions/1842987200/

  
# Course-Schedule-II
- Donot forget to check for cycle after getting topo order of courses .
- KEEP IN MIND : Kahn's algo (a,b) where a says go do b first then indeg of b in inc and b->a graph formed , but in DFS we do the rev a->b and do a post order dfs ie for a we do and visit all its nbr
- TC : O(V+E) ie because for all V nodes all e edges are checked no matter we get another v node or not ? , SC = O(V+E) -> adj list 
- DO : https://leetcode.com/problems/course-schedule-ii/

# Parallel courses-III
- DP + Topological Order , TC = O(V + E) , SC = O(V + E)
- https://leetcode.com/problems/parallel-courses-iii/submissions/1876409560/

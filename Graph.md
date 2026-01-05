# Course-Schedule-II
- Donot forget to check for cycle after getting topo order of courses .
- KEEP IN MIND : Kahn's algo (a,b) where a says go do b first then indeg of b in inc and b->a graph formed , but in DFS we do the rev a->b and do a post order dfs ie for a we do and visit all its nbr
- TC : O(V+E) ie because for all V nodes all e edges are checked no matter we get another v node or not ? , SC = O(V+E) -> adj list 
- DO : https://leetcode.com/problems/course-schedule-ii/

# UNIQUE PATHS 3 :
- ` TC : O(3^(n*m)) `  :BRACNKING FACTOR OF 3 is every cell has 4 cardinal directions and one of those is the direction we came from to the curr cell so visited , hence further 3 more directions to explore
- - Theoretically is 3^(n*m) but as blocked cell and dead ends will occur then this DFS + BACKTRACKING approach works better than DP+Bitmask {as dp memory allocation is time consume for all states of visited cells} - BACKTRACKING PRUNING {ie cutting off invalid paths early} WORKS WONDERS {make it more efficient than DP+Bitmask}
- SC = O(N*M) {Recursive stack and vis arr} 
- DO : https://leetcode.com/problems/unique-paths-iii/


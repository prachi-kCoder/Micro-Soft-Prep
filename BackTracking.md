# RAT IN A MAZE ;
- DO :https://www.geeksforgeeks.org/problems/rat-in-a-maze-problem/1
- take O(N x N)->Recusion stack space ,  O(1) extra space using the same matrix for modifications , donot make visited mat separately
- TC = O(3^NxN)  as branching factor for all nxn cells will be 3 directions (exclusing the 1 from which we came over over the cell !) 

# M-COLORING
- Its a NP-complete problem 
- `TC= O(M^V) M-> no of colors , V->vertices` to be precise O(M^V * V) because M  colors over all v vertices M X M X m.. v times hence M^v and for assigning colors is_safe pruning is applies that lower down the recursion call
- But for dense graphs , then all edges all other v neighbours connect so is_safe iteration over all nbs => O(V)  ,
- is_safe optimisation optimises but worst case complexicity remain exponential
- DO :https://www.geeksforgeeks.org/problems/m-coloring-problem-1587115620/1

  
# UNIQUE PATHS 3 :
- ` TC : O(3^(n*m)) `  :BRACNKING FACTOR OF 3 is every cell has 4 cardinal directions and one of those is the direction we came from to the curr cell so visited , hence further 3 more directions to explore
- - Theoretically is 3^(n*m) but as blocked cell and dead ends will occur then this DFS + BACKTRACKING approach works better than DP+Bitmask {as dp memory allocation is time consume for all states of visited cells} - BACKTRACKING PRUNING {ie cutting off invalid paths early} WORKS WONDERS {make it more efficient than DP+Bitmask}
- SC = O(N*M) {Recursive stack and vis arr} 
- DO : https://leetcode.com/problems/unique-paths-iii/

# NQUEENS :
- Here ldia, rdia , cols works as we take the blocked positions collective & its ~ is the safe positions then safe position take by getting rightmost set bit from safe mask and then , cols with c used , and c marked in ldia and set it leftshift rightly to know leftdia ->marking its cells down in row, same is the case in rightdia ->mark its cell down in rows ;
- Do :https://www.geeksforgeeks.org/problems/n-queen-problem0315/1
- tc : O(N!) , sc = O(N) rec stack space 

# Partition to K equal sum subsets
- Do :https://leetcode.com/problems/partition-to-k-equal-sum-subsets/submissions/1878642896/
- Keep in mind pruining make this to work more efficiently better than O(K^N)
- `DESCENDING PRUING` : TO FILL IN BUCKET FAST WITH LARGE VALUES
- `SAME STATE PRUNING` : TO AVOID EXPLORING SAME STATE
- `EMPTY BUCKET PRUNING` : TO KNOW IF EMPTY BUCKET ALLOCATION WASN'T SUCCESSFUL SO NO POSSIBLE FOR ANY OTHER ALLOCATION
- `EXACT MATCH PRUNING` : IF EXACT MATCH FOUND , BEST ALLOCATION THEN CAN'T BE FEASIBLE WITH ANY OTHER ALLOCATION
  
# SUBSET-II
- `j > si & nums[j-1] == nums[j]` this condition is necessary for proning as we want to avoid start the tree with duplicate occ on same recursion level , ## SORTING ## is a must -> As duplicate elements should come adjacently to skip them !
- TC = O(N * 2^N + N logN )  : as 2^N subsets formation , copying n elements of subsets in ans take O(n) at each recursive level
- SC = O( N  + N * 2^N) for output of O(N* 2^N) + O(N) ie the recursion stack
- Do : https://leetcode.com/problems/subsets-ii/

# Palindrome-Partition
-  O(n) work for each of the 2^n valid partitions, the total complexity is O(n*2^n) , worst case will be a string of all same character where each partition reached the right space ! & SC = O(N + N* 2^N)
-  Do : https://leetcode.com/problems/palindrome-partitioning/

  

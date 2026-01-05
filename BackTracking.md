# UNIQUE PATHS 3 :
- ` TC : O(3^(n*m)) `  :BRACNKING FACTOR OF 3 is every cell has 4 cardinal directions and one of those is the direction we came from to the curr cell so visited , hence further 3 more directions to explore
- - Theoretically is 3^(n*m) but as blocked cell and dead ends will occur then this DFS + BACKTRACKING approach works better than DP+Bitmask {as dp memory allocation is time consume for all states of visited cells} - BACKTRACKING PRUNING {ie cutting off invalid paths early} WORKS WONDERS {make it more efficient than DP+Bitmask}
- SC = O(N*M) {Recursive stack and vis arr} 
- DO : https://leetcode.com/problems/unique-paths-iii/

# SUBSET-II
- `j > si & nums[j-1] == nums[j]` this condition is necessary for proning as we want to avoid start the tree with duplicate occ on same recursion level , ## SORTING ## is a must -> As duplicate elements should come adjacently to skip them !
- TC = O(N * 2^N + N logN )  : as 2^N subsets formation , copying n elements of subsets in ans take O(n) at each recursive level
- SC = O( N  + N * 2^N) for output of O(N* 2^N) + O(N) ie the recursion stack
- Do : https://leetcode.com/problems/subsets-ii/

# Palindrome-Partition
-  O(n) work for each of the 2^n valid partitions, the total complexity is O(n*2^n) , worst case will be a string of all same character where each partition reached the right space ! & SC = O(N + N* 2^N)
-  Do : https://leetcode.com/problems/palindrome-partitioning/

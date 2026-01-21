# Kth smallest ele :
- do :https://leetcode.com/problems/kth-smallest-element-in-a-sorted-matrix/submissions/1886452392/
- Assume mat as klist of array and get the smallest k-1 processed TC : O(Klog(N)) , SC= O(K)
- OR binary search STAIRCASE APPROACH ! O(N * LOG M) , M->max element range 
  
# SHORTEST PATH IN GRID ;
- if K>=m+n-3  then enough obstacle as 1st and last cells are ob free so just take the shourtes path of m+n-2 move m-1 downs and n-1 rights
- PTS :`bfs` for shortest path , `obstacle should be there with every entry in q` , `vis[][] to keep that how many K left to use for obstacle destruction` , TC = O(M X N  xK)
- Only allow if the vis[i][j] is high ie another path revisiting the cell then should have more destruction power for ob , is it will include more steps as in BFS baad me aaya so should only consider if have advantage associated !
- Do:https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/submissions/1883501840/

# revise these :https://leetcode.com/discuss/post/7374749/20-binary-search-problems-to-revise-befo-hbtt/?utm_source=copilot.com

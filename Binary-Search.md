# K-SUBARRAY-SUM
- Revise it one using prefix_sum , unordered_map to know can we get ( curr_sum - k ) as a prefix sum on the left to exclude so we get the subarray sum = k
- Do : https://leetcode.com/problems/subarray-sum-equals-k/submissions/1882738744/
  
# Kth smallest pair
- Do : https://leetcode.com/problems/find-k-th-smallest-pair-distance/description/?envType=problem-list-v2&envId=7p5x763
- TC : O(MLOGM + NlogN) where M-> max_diff O(1)sc 

# single ele : sorted array o(logn)
- get the positing of mid,  mid^+1 the if = then eliminate it otherwise keep is high = mid ;
- do : https://leetcode.com/problems/single-element-in-a-sorted-array/submissions/1898332731/
  
## BINARY-SEARCH IN 2D MATRIX
`IF ROWWISE + COLWISE SORTED + ROW&COL IN ORDER `:
- {take the matrix as flattened arr 0,m x n-1} 
- do :https://leetcode.com/problems/search-a-2d-matrix/description/

` if ROWWISE + COLWISE SORTED but not in order`
- BINARY SEARCH AS PER THE VALUES , + staircase approach !
  
` if only rowwise sorted` 
- Binary search over values but staircase won't work here ,so individually perform binary search over rows {as only those are sorted}
- Do:https://www.geeksforgeeks.org/problems/median-in-a-row-wise-sorted-matrix1527/1

 
- Binary-Search 
# median of 2 sorted array when merged 
- Keep in binary search over smaller array and mid1 os the contribution len on left of med
- So low = 0 , high = n {not the indices they are length contributed} and len = (n+m+1)/2 ; as for odd ans is on left side
- Do :https://leetcode.com/problems/median-of-two-sorted-arrays/submissions/1875140710/

# Peakele1 :
- arr[mid] , arr[mid+1] , these 2 element are enough to know the slope of values 
- DO:https://www.geeksforgeeks.org/problems/peak-element/1?amp%3Butm_campaign&utm_source=geeksforgeeks&%3Butm_medium=ml_article_practice_tab
# Peak-Element2 :
- KEEP YOUR FOCUS ON how  moveing through global maximam in a col ensures that the value remain greater than any value on its left/right than it ensure either ends to reach the end cell of the row or you get the peak ! TC = O(M logN)  SC = O(1)
- Do :https://leetcode.com/problems/find-a-peak-element-ii/
# TWO - POINTERS {not binary search}

# 3SUM :
- https://leetcode.com/problems/3sum/submissions/1882687809/
- O(N^2)
- Or better try this :https://leetcode.com/problems/3sum-closest/
- tc = O(N^2) keep in mind !! as we are applying two pointer approach no the binary search here we just look at high and low and increment or decrement the pointers whether we get higher value or lower based on that we move on low or on high ! , we aren't moving as low++ , high-- so the search space is not decresing by 1/2 !! so it 2 ptr!

# 4SUM :
-TC = O(N^3)
-do : https://leetcode.com/problems/4sum/submissions/1883630219/

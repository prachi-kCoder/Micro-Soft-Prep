# K-SUBARRAY-SUM
- Revise it one using prefix_sum , unordered_map to know can we get ( curr_sum - k ) as a prefix sum on the left to exclude so we get the subarray sum = k
- Do : https://leetcode.com/problems/subarray-sum-equals-k/submissions/1882738744/
  
# 3SUM :
- https://leetcode.com/problems/3sum/submissions/1882687809/
- Or better try this :https://leetcode.com/problems/3sum-closest/
- tc = O(N^2) keep in mind !! as we are applying two pointer approach no the binary search here we just look at high and low and increment or decrement the pointers whether we get higher value or lower based on that we move on low or on high ! , we aren't moving as low++ , high-- so the search space is not decresing by 1/2 !! so it 2 ptr!


- Binary-Search
# median of 2 sorted array when merged 
- Keep in binary search over smaller array and mid1 os the contribution len on left of med
- So low = 0 , high = n {not the indices they are length contributed} and len = (n+m+1)/2 ; as for odd ans is on left side
- Do :https://leetcode.com/problems/median-of-two-sorted-arrays/submissions/1875140710/

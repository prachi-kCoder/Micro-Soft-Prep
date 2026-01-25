# Rotated-Sorted-Types

## B-Seach for target :
- find which part is sorted , then move towards it ,
- If `LEFT HALF IS SORTED ` :nums[low] <= nums[mid] ,
- ELSE : `RIGHT HALF IF SORTED` ; Using sorted range check target their in sorted increasing range and make movement accordingly !
- O(log N) : https://leetcode.com/problems/search-in-rotated-sorted-array/description/
- With duplicates just skip the range if l,mid,h all same so l++ , h-- : https://leetcode.com/problems/search-in-rotated-sorted-array-ii/


# GET-MIN ;
- compare mid to high if mid is lesser be on left , but low < high wala Bsearch is keep mid as well in case nums[mid] <= nums[high] :
- Do :https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/submissions/1896424008/

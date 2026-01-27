# Rotated-Sorted-Types

## B-Seach for target :
- find which part is sorted , then move towards it ,
- If `LEFT HALF IS SORTED ` :nums[low] <= nums[mid] ,
- ELSE : `RIGHT HALF IF SORTED` ; Using sorted range check target their in sorted increasing range and make movement accordingly !
- O(log N) : https://leetcode.com/problems/search-in-rotated-sorted-array/description/
- With duplicates just skip the range if l,mid,h all same so l++ , h-- : https://leetcode.com/problems/search-in-rotated-sorted-array-ii/


# GET-MIN ;
- arr[mid] > arr[high] says sorted arr is rotated and initial part having min element would obviously on right , else on left !
- Do :https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/submissions/1896424008/

# peak element :
- here arr[mid] & arr[mid+1] is compare as high can be smaller peak can be anywherr in array : https://leetcode.com/problems/peak-index-in-a-mountain-array/
# GEt complete range of target 
- https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/submissions/1898425124/

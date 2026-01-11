# Smallest sufficient team ;
- TC : O(N x (1<<M))  where n= no. of people ,K->total skills 
- DO :https://leetcode.com/problems/smallest-sufficient-team/submissions/1881747950/

# SUBSET - ENUMERATION :
- submask of mask is mask by the loop : TC = (3^n)  
- `submask = mask ; submask > 0 ; submask = (submask-1)& mask`  why so ? because for submask , here mask act as a filter to ensure bit with 1's are only considered !
- Do minTime for jobs : https://leetcode.com/problems/find-minimum-time-to-finish-all-jobs/description/
- tc : 3^N
- Do : parallel courses :
- tc :
- Do Number of valid words : https://leetcode.com/problems/number-of-valid-words-for-each-puzzle/submissions/1881863782/
- tc : O(N * L + M * 2^{K-1}) all mask are no enumerated for submask only (1<<6) are enumerated !
- {This ques can also be done using BinarySearch Backtracking with pruning }

# SINGLE NO-3 
- {2 unique nos .}GROUP DIVISION : look for right most set bit `unsigned int diff_bit = (unsigned int) x ^ -(unsigned int)x`; here first type case then put(-) ie -(unsigned int) x  , to prevent Undefined behaviour of as 0 is included in non negative side `[-2^31 , 2^31-1]` .
- Do : https://leetcode.com/problems/single-number-iii/submissions/1877207598/
  
# single no 2 ;
- tc = O(N) , SC = O(1)
- DO : https://leetcode.com/problems/single-number-ii/

# Cnt bits : 
- revise:https://leetcode.com/problems/counting-bits/submissions/1877366183/


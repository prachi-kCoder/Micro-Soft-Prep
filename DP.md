# OPPONENT STRATEGY FOR GAME :
- Keep in mind MINMAX strategy ie {don't confuse it with that you want to min the opponent's score} , but its considering that you made the a choice and get the min of the next choice as the opponent is also playing optimally and take the max of those 2 turns :
- `left + min(rest ranges for next you own turn) , right + min(rest range of your next turn )`
- DO (1D- dp optimisation!) : https://www.geeksforgeeks.org/problems/optimal-strategy-for-a-game-1587115620/1

# MIN-DIFF PARTIOTION:
- Your thought it right to reach target/2 so minimise the diff between the 1st half <= totalsum/2 and 2nd half = total_sum-1st_half
- Just use  1D bool DP , or rather use bitset {allows u to make state for 1e5 member {don't always think of make bitmask , bitset allowsfor tabulation apporach}}
- Do : https://www.geeksforgeeks.org/problems/minimum-sum-partition3317/1

# Work-Break
{It actually depends upon the len of string and word_dict whether to iterate more on dict or on string}
{If size(dict) < len(s)} :-
- DO :https://www.geeksforgeeks.org/problems/word-break1352/1
{If size(dict) > len(s)} :-
- DO : https://leetcode.com/problems/word-break/submissions/1872268075/
# Word Break ii
- Do : https://leetcode.com/problems/word-break-ii/submissions/1872638660/
  
 # MIN-PATH-SUM in grid
 - don't forget the browny point of Space optimisation : O(M) rather that making O(N x M) dp table :
 -  Do  :https://leetcode.com/problems/minimum-path-sum/description/

# INTERLEAVE STRINGS : 
-DO 1d optimised version by restricting the sp to 1 dimension , jth one only !
- Do here : https://www.geeksforgeeks.org/problems/interleaved-strings/1

## MCM -> 2 variations : 
- 1) MCM STANDARD WITH MiniCost Split : dp[i][k] , dp[k+1][j] , curr cost arr[i-1] ,arr[k] ,arr[j] dependent or sometimes on conditions
  TRY ON : https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/ 
  3) BURST BALLOON : dp[i][j] = dp[i][k-1] , dp[k+1][j] ie kth is the last which was removed that variation is based on this ! , {inverse intution of k was removed -> solve it assuming it the last one to be removed !}
     
  - MAX-SKILL/ BURST-BALOON : MCM but reconstruction ! to max not to min
- Do here : https://www.geeksforgeeks.org/problems/burst-balloons/1   ,
- or @ : https://leetcode.com/problems/burst-balloons/description/

- For each interval (i, j), we try every possible balloon k as the last one to burst, combining results from left and right subintervals dp[i][j] -> max of all k from [i,j] with dp[i][j] = dp[i][k-1] + dp[k+1][j] + arr[i-1] * arr[k] * arr[j+1]
- TC = O(n^3)


# EGG-DROP :
- intuitive approach of `e v/s floor dp to get CNT OF min moves` : Give tle though O(E *F * F)
- Optimise with inverse DP `e v/s moves dp to get the cnt of floor to atleast reach = f` : O(E * M) , where M -> no. of moves for ie log2(F)
- final optimal answer is 1D dp with `egg v/s moves variation` O(E*M) , M =LOG2(F)
- Do it : https://www.geeksforgeeks.org/problems/egg-dropping-puzzle-1587115620/1

# Super Seq (using lcs) reconstruction also !
- TC = O(n*m) , SC => O(M) {Get the most optimised version !} but the O(N*M) necessary for LCS reconstruction!
- DO : https://www.geeksforgeeks.org/problems/shortest-common-supersequence0322/1


```cpp
1D DP OPTIMISATION :
- FIRST LOOK AT HOW DP IS DEFINED {IF THE INTERVAL DP IS LENGTH BASED ie the outer loop of 2D dp is LEN } :
- The Interpretation of i, prev, and prev_prev  :
` len: This is the size of the current subproblem (the number of elements in the range).
- i: This is always the starting index of the current range.
- curr[i]: Represents the result for the range starting at i with length len. (The end index is implicitly j = i + len - 1).
- prev[i]: Represents the result for a range starting at i with length len - 1.
- prev_prev[i]: Represents the result for a range starting at i with length len - 2
look at len then check the starting index for the curr in recurrence only!

- IF the DP is range based of indexes {i to j} then : Check in this types here usually only 1 dp works : well :https://www.geeksforgeeks.org/problems/interleaved-strings/1
```
# Longest palindromic subsequence 
- O(N) optimisation of space is by making use of DP1d base on len : prev , prev_prev made prev-> of len-1 , prev_prev->len-2
- DO: https://leetcode.com/problems/longest-palindromic-subsequence/submissions/1877761465/

# EDIT DISTANCE : 
- Here the DP 1d optimisation is more on the (i) row based ie the outer loop is of {unlike the Longest palindromic Sub where the outloop is of len so prev row is of len-1,  prev_prev is of len-2} , but here i is in outer loop so prev_row is of values of (i-1)th row
- Get SC(O(M)) , TC = O(N+M) & donot forget making init : https://leetcode.com/problems/edit-distance/description/ 

# ROD-CUTTING
- Do initialised with dp[i] = price[i-1] to consider the complete length as well
- Do:https://www.geeksforgeeks.org/problems/rod-cutting0840/1

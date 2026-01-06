

# Work-Break
{It actually depends upon the len of string and word_dict whether to iterate more on dict or on string}
{If size(dict) < len(s)} :-
- DO :https://www.geeksforgeeks.org/problems/word-break1352/1
{If size(dict) > len(s)} :-
- DO : https://leetcode.com/problems/word-break/submissions/1872268075/
# Word Break ii
- Do : https://leetcode.com/problems/word-break-ii/submissions/1872638660/


# INTERLEAVE STRINGS 
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

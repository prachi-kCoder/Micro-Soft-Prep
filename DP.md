
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


# MAX-SKILL/ BURST-BALOON : MCM but reconstruction ! to max not to min
- For each interval (i, j), we try every possible balloon k as the last one to burst, combining results from left and right subintervals dp[i][j] -> max of all k from [i,j] with dp[i][j] = dp[i][k-1] + dp[k+1][j] + arr[i-1] * arr[k] * arr[j+1]
- TC = O(n^3)
- Do here : https://www.geeksforgeeks.org/problems/burst-balloons/1
- 
# EGG-DROP :
- intuitive approach of `e v/s floor dp to get CNT OF min moves` : Give tle though
- Optimise with inverse DP `e v/s moves dp to get the cnt of floor to atleast reach = f` :
- final optimal answer is 1D dp with `egg v/s moves variation`
- Do it : https://www.geeksforgeeks.org/problems/egg-dropping-puzzle-1587115620/1

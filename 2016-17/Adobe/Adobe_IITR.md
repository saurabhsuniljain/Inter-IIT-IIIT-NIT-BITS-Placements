# Coding Round (3 questions)
1. Given a string containing only ‘+’ and ‘-’, find the length of the longest substring containing only ‘+’.
2. Given a word list and a sentence determine the least cost of generating the sentence from the words given in the list. A valid sentence is a combination of 1 or more words without any spaces and can contain any permutation of the words. Eg if list contain “abc” then the sentence can contain “abc”, “cab”, “bac”, etc. The cost is defined as the number of places where the word in the sentence and the corresponding word in the list differ from each other. Eg if list has abc and sentence contains a substring “cab” then the cost  = 3. Assumptions : You can use the same word multiple times and any transformation each time you use it. Assumed Constraints : 1 < |s| < 5000 [Passed all test cases].
3. Problem : There are n people numbered 1 to n. Some people are enemy, such pairs are given. You can form a group from range X to Y (from person numbered X to person numbered Y, all included) if and only if there is no pair (i,j) between X and Y such that (i,j) is enemy. Find how many total groups you can form. Constraints : 1 <= N, M <= 10^6.

#Solutions
1. Trivial (Find all substrings and print maximum)
2. 
3. Approach : DP (store for each person till how far he can from the group). 

    dp[i] = min(dp[i+1], next_enemy(i))

    next enemy is the first enemy of i after index i. [Can be found in O(n) time overall - assign all next[i] to n+1, now process each pair of enemy (i,j) if j>i update next[i] = min(next[i],j) else update next[j] = min(next[j],i) ]

    Final answer : After calculating dp array, do summation of (dp[i] - i) for i = 1 to N.

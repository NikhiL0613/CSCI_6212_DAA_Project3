Pseudo-polynomial Partition
Given a set consisting of n integers [a1, a2, … an], you want to partition into two parts so that the sum of the two parts is equal.  Suppose s = a1 + a2 … + an. The time complexity of your algorithm should be O(ns) or better.


The idea is to use dynamic programming (DP) to solve the partition problem. We begin by calculating the total sum s of the integers in the set; if s is odd, an equal partition is impossible. If s is even, we set the target sum to s/2 and seek to determine if there exists a subset of elements that sums to this target. The DP table dp[i][j] indicates whether a subset sum j can be achieved using the first i elements of the array, where we update the table based on including or excluding each element. This approach runs in O(ns) time, where s is the total sum, making it a pseudo-polynomial solution suitable for moderate values of n and 

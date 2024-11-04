(i) Illustration of Asymptotic Notations in Algorithm Analysis 

Asymptotic notations are mathematical tools used to describe the behavior of an algorithm’s time or space complexity as the input size grows. They help to evaluate and compare the efficiency of algorithms by focusing on the rate of growth of the runtime or memory requirement rather than specific runtime values.

Key Asymptotic Notations:
1. Big O Notation (O):
  a. Describes the upper bound of an algorithm's runtime, providing a worst-case scenario.
  b. Example: If an algorithm takes at most c.n^2 operations for some constant c we express the complexity as O(n^2)
, meaning the runtime will not grow faster than n^2.


2.Omega Notation (Ω):

Describes the lower bound of an algorithm's runtime, representing the best-case performance.
Example: If an algorithm takes at least 
𝑐.𝑛
c⋅n operations, then it has a complexity of 
Ω(n), implying that in the best case, the runtime grows no slower than n.

3.Theta Notation (Θ):
Describes the tight bound of an algorithm, representing both the upper and lower bounds. It indicates that the algorithm’s runtime grows at exactly this rate.
Example: If an algorithm takes exactly 
𝑐⋅𝑛 operations in all cases, then its complexity is 
Θ(n),implying the runtime is proportional to n.

Application in Algorithm Analysis:
Using these notations, we can analyze an algorithm's performance:

Example: For a simple loop iterating 
n times, the runtime complexity can be expressed as 
𝑂(𝑛)because it grows linearly with 𝑛.
Comparing Algorithms: Suppose we have two algorithms, one with 
𝑂(𝑛)complexity and another with 
𝑂(𝑛^2)
O(n^2). For large inputs, the 
𝑂(𝑛) algorithm will be more efficient as its runtime increases more slowly.
 
 Asymptotic analysis, therefore, gives a framework for comparing the efficiency of algorithms, regardless of machine-dependent factors, by analyzing how the algorithm scales with larger inputs.

 (ii) Time and Space Complexity Analysis for the Given Code:

 
#include <stdio.h>
int main() {
    int i = 1, sum = 0, n;
    while (i <= n) {
        i = i + 1;
        sum = sum + i;
    }
}

Time Complexity:
1.Loop Analysis: The while loop runs as long as i <= n. Inside the loop, i is incremented by 1 in each iteration, so the loop runs approximately 
n times.

2.Operations Per Iteration: In each iteration, the loop performs:
a.Increment operation (i = i + 1) - constant time, 
O(1).
b.Addition operation (sum = sum + i) - constant time, 
O(1)

Since both operations inside the loop take constant time 
𝑂(1), the total time complexity is determined by the number of loop iterations, which is 
n. 
Therefore, the time complexity is:
O(n)

Space Complexity:
1.Variable Storage: The code uses a fixed amount of memory to store three integers (i, sum, and n), regardless of the input size n. These require constant space.
Since no additional space is used that depends on n, the space complexity is:O(1)

Summary:

1.Time Complexity: O(n)
2.Space Complexity: O(1)











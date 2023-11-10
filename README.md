# CSCI--CQ7

Space and time complexity analysis of Running time of algorithms

Time Complexity
Outer Loop (for-loop) Iterates n-1 times where n is the size of the array.
Inner Loop (while-loop): Iterates i times for each iteration of the outer loop.
Taking this into account the time complexity is O(n^2)

Space Complexity
Input Size: The size of the input array is `n`.

Therefore, the space complexity is O(1) (constant space complexity)


Ice Cream Parlor Recursive Definition
The function returns a pair of indices if it finds two distinct flavors that add up to the initial total amount.

Base Case:
   - If `i` is equal to the length of `arr`, return an indication that no valid pair was found

Recursive Step
   - For the current index `i`, check if there exists another index in the array such that arr[i] + arr[j] == m.
   - If such a j is found, return the pair of indices (i, j).
   - If not, recursively call findFlavors(i + 1, m, arr) to check the next index.


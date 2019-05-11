# Add your answers to the Algorithms exercises here.
## Exercise I
a) The first line is 0(1), the second line is dependent on how a iterates. The third line shows that a iterates at n squared. Hence, the second line is 0(n). Since, 0(n) is worst case that is the time complexity.

b)  line 1 -> O(1)
    line 2 -> O(n)
    line 3 -> O(n) * O(nlogn)
    line 4 -> O(n) * O(nlogn)^2
    line 5 -> O(n) * O(nlogn)^2 * O(10n)
    since O(n) ~ O(nlogn),
    worst case for time complexity -> O(n^4)  

c) We'll assume the bunnies parameter in this equation is n for the sake of understanding. Since this is a recursive function that calls itself until the base case is reached and drops 1 n per recursion, the time complexity is O(n).

## Exercise II
Since the stories in this building are sorted from lowest to highest, we can use a binary search to find floor _f_. This search would go to the middle of the building and drop an egg. If the egg breaks, the search would go to the middle of the lower half of the building and drop an egg there. If the egg does not break, the search would go to the upper half of the building and drop an egg. This would be repeat until we find floor _f_, where an egg breaks but no floors below it break the egg. 
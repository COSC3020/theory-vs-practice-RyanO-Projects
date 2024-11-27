# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Asymptotic notation focuses on time complexity over other potentially important factors like space complexity. Suppose an algorith has an extremely fast run-time but is very inefficient with the amount of memory it uses. This algorithm may work just fine on most computers but consider the case in which you have a computer with extremely limited extra memory. Although the asymptotic analysis tells us that the algorithm would theoretically be the best choice, the limitations imposed by our computer make it impractical or even impossible to implement.
    2. Depending on which form of asymptotic notation you used for your algorithm it can give a misleading runtime compared to the actual runtime based on the variability of the input. For example, if we say that the runtime of intsertion sort is $O(n^2)$ but the input array is already sorted it will result in an actual runtime analysis of $O(n)$, a drastic difference between the theorized and actual runtime results.
    3. The asymptotic analysis may also be misleading in that it is mainly concerned with very large values of n. While two different algorithms may have runtimes of $\Theta(nlog(n))$ and $O(n)$, on paper it would seem that the first algorithm is the much more attractive option, however at smaller values of n the runtime difference is almost negligible such that it might not even make a difference which algorithm you decided to implement.
       
- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.
    1. We know that search time of a binary search tree is dependent on the height of the tree. Assuming that the binary search tree is balanced, we can infer that the height of the 1,000 element tree is $log_2(1000)$ or ~10. Assuming the binary search tree with 10,000 elements is also balanced then the height of that tree would be $log_2(10000)$ or ~13. Since the height determines the search time, we can estimate the search time of the larger tree by comparison.. If it takes 5 seconds to search a binary tree of depth 10, then we can find the calculation for the search time of a binary search tree of depth 13 by multiplying the search time of the 1,000 element tree by the scalar of the two trees, $(13/10) * 5 = 6.5$ seconds.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.
    1. It could be that the search tree isn't balanced leading to a more linear runtime than the logarithmic runtime we would typically expect.
    2. It could also be 

Add your answers to this markdown file.

https://iq.opengenus.org/time-and-space-complexity-of-binary-search-tree/

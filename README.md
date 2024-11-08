# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
    1. Asymptotic notation focuses on time complexity over other potentially important factors like space complexity. Suppose an algorith has an extremely fast run-time but is very inefficient with the amount of memory it uses. This algorithm may work jjust fine on most computers but consider the case in which you have a computer with very limited extra memory. Although the asymptotic analysis tells us that the algorithm would theoretically be the best choice, the limitations imposed by our computer make it impractical or even impossible to implement.
       to run on has extremely limited memory. 
- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

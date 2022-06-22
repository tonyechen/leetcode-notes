# Topics I need to practice:
* Linked Lists


## Space Complexity
Total amount of memory space used by an algorithm/program including the space of input values for execution

Space Complexity = Auxiliary space + Space use by input values
* O(1) (constant space, a fixed number of variables, doesn't scale with argument)
* O(N) (scale with argument, usually like arrays or similar datatypes)

# Algorithms
## Greedy Algorithms
---
A greedy algorithm is an approach for solving a problem by selecting the best option available at the moment. It doesn't worry whether the current best result willl bring the overall optimal result.

It works in a top-down approach and nevever reverses the earlier decision even if the choice is wrong. 
1. Greedy Choice Property
    - an optimal solution to the problem can be found by choosing the bets choice at each step without reconsidering the previous teps once chosen, the peoblem can be solved using a greedy approach
2. Optimal Substrucutre
    - if the optimal overal solution to the problem corresponds to the optimal solution to its subproblems, then the problem can be solv3ed using a greedy approach

## Dynamic Programming
---
A technique in computer programming for solving a given complex problem by breaking it down into subproblems and memorizing the outcomes of those subproblems to prevent repeating computations

Properties of Dynamic Programming
1. Optimal Substructure
    - a problem is said to have an optimal substructure if we can formulate a recurrence relation for it
2. Overlapping subproblem
    - A problem is said to have an overlapping subproblem if the subproblems reoccur when implementing a solution to the larger problem

Tabulation vs Memoization

Tabulation = Bottom Up Approach, create a 2D array

Memoization = Top down Approach, memorize a value at a time

## Kadane's Algorithm:
---
Solving Maximum Subarray Problems


link: https://medium.com/@rsinghal757/kadanes-algorithm-dynamic-programming-how-and-why-does-it-work-3fd8849ed73d

# Data Structures

# Computational techniques
## Sliding Window
https://www.geeksforgeeks.org/window-sliding-technique/

aims to reduce the use of nested loop and replace it with a single loop, thereby reducing the time complexity

pre-requisite:
- can only be used in a very specific scenario, where the size of window for computation is fixed throughout the complete nested loop, Only then the time complexity can be reduced.

General Idea: Calculate a section of an array, then slide the section over by a fixed number of elements, subtract the old items and add the new items.
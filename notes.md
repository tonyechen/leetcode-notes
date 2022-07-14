# Topics I need to practice:
- Linked Lists
- Dynamic Programming
- Greedy Algorithm

## Top 100 liked question set (order from easy to hard):
Link: https://leetcode.com/problem-list/top-100-liked-questions/?sorting=W3sic29ydE9yZGVyIjoiQVNDRU5ESU5HIiwib3JkZXJCeSI6IkRJRkZJQ1VMVFkifV0%3D
# Notes
## Space Complexity
Total amount of memory space used by an algorithm/program including the space of input values for execution

Space Complexity = Auxiliary space + Space use by input values
* O(1) (constant space, a fixed number of variables, doesn't scale with argument)
* O(N) (scale with argument, usually like arrays or similar datatypes)

# Algorithms
## Greedy Algorithms
---
A greedy algorithm is an approach for solving a problem by selecting the best option available at the moment. It doesn't worry whether the current best result willl bring the overall optimal result.

It works in a top-down approach and never reverses the earlier decision even if the choice is wrong. 
1. Greedy Choice Property
    - an optimal solution to the problem can be found by choosing the bets choice at each step without reconsidering the previous teps once chosen, the peoblem can be solved using a greedy approach
2. Optimal Substrucutre
    - if the optimal overall solution to the problem corresponds to the optimal solution to its subproblems, then the problem can be solved using a greedy approach

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
Solving Maximum Subarray Problems

link: https://medium.com/@rsinghal757/kadanes-algorithm-dynamic-programming-how-and-why-does-it-work-3fd8849ed73d


## Floyd's Cycle Finding Algorithm (Tortoise-Haire Algorithm)
----
A pointer algorithm that only uses two pointers, moving through the sequence and different speeds. This algorithm is used to find a loop inside a linked list with O(n) time and O(1) space, but can also be adapted to solve other problems like finding duplicates inside a list.

Link: https://www.geeksforgeeks.org/floyds-cycle-finding-algorithm/#:~:text=How%20Does%20Floyd's%20Cycle%20Finding%20Algorithm%20Works%3F&text=The%20Fast%20pointer%20may%20reach,exists%20in%20the%20linked%20list.

## Boyer-Moore Voting Algorithm
---
one of the most popular optimal algorithms used to find the majority element among the given elements that have more than N/2 occurences.

It workds on the fact that if an element occurs more than N/2 times, it means that the remaining elements other than this would definitely be less than N/2:
- First, choose a candidate from the given set of elements if it is the same as the candidate element, increase the votes. Otherwise, decrease the votes if votes become 0, select another new element as the new candidate. 
- if it is not given that majority element exists, we must loop through the array again and count the occurences of candidates to make sure that it is a majority element
### Intuition Behind Working:
Why can we disregard the prefix elements? Because we have more majority elements than the minority elements, so by disregarding prefixes, we are ignoring an equal amount of majority and minority elements, therefore, the majority element will still be the majority element in the following elements after we throw away the prefixes. We will eventually run out of minority elements but will still have majority element. And we cannot discard more majority elements than minority elements.

Link: https://leetcode.com/problems/majority-element/solution/
# Data Structures

# Computational techniques
## Sliding Window
https://www.geeksforgeeks.org/window-sliding-technique/

aims to reduce the use of nested loop and replace it with a single loop, thereby reducing the time complexity

pre-requisite:
- can only be used in a very specific scenario, where the size of window for computation is fixed throughout the complete nested loop, Only then the time complexity can be reduced.

General Idea: Calculate a section of an array, then slide the section over by a fixed number of elements, subtract the old items and add the new items.

## Two Pointers:
---
## Two runners pointer technique:
Imagine we have 2 runners one fast and one slow, running down the nodes of the Linked List. In each second, the faster runner moves down 2 nodes, and the slow runner just 1 node, By the time the faster runner gets to the end of the list, the slower runner will be half way. By representing the runners as pointers, and moving them down the list at the coreesponding speeds. we can use this trick to find the middle of the list.

## Tail Recursion
A specific form of recursing where the recursive call is the last action in the function. The benefit of tail recursion is that for certain programming languages such as c++ the complier could optimize the memory allocation of call stack by reusing the same space for every recursive call, rather than creating the space for each one, allowing one to obtain the constant space complexity O(1) for the overhead of the recursive calls.
- not supported by python or java

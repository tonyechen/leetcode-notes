# Topics I need to practice:
* Linked Lists


## Space Complexity
Total amount of memory space used by an algorithm/program including the space of input values for execution

Space Complexity = Auxiliary space + Space use by input values
* O(1) (constant space, a fixed number of variables, doesn't scale with argument)
* O(N) (scale with argument, usually like arrays or similar datatypes)

# Algorithms

# Data Structures

# Computational techniques
## Sliding Window
https://www.geeksforgeeks.org/window-sliding-technique/

aims to reduce the use of nested loop and replace it with a single loop, thereby reducing the time complexity

pre-requisite:
- can only be used in a very specific scenario, where the size of window for computation is fixed throughout the complete nested loop, Only then the time complexity can be reduced.

General Idea: Calculate a section of an array, then slide the section over by a fixed number of elements, subtract the old items and add the new items.
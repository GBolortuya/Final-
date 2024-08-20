# Final-
Python - Max Heap Implementation and Application

I. Introduction

As mentioned above  , the PriorityQueue  has some problems. The underlying principle of priority queue sorting is based on Max Heap. Let's take a look at the basic implementation and usage of Max Heap . First, let's clarify the concepts related to Max Heap and its implementation:

A. A maximum heap, also known as a large root heap (large top heap), means that the value of the root node (also called the top of the heap) is the largest value among all the nodes in the heap.

(1) The value of each root node is greater than that of its leaf nodes

(2) A maximum heap is a complete binary tree

B. Complete binary tree, a binary tree with a depth of k and a number of nodes of 2^k - 1 is a complete binary tree

(1) Find the parent node given an index


(2) Find child nodes given an index

2.Maximum heap implementation
  
 1. Initialization
      
 (1) maxSize is the initialization array length of the maximum heap

 (2) count is the number of elements in the current maximum heap
    
 (3) The show function returns the current array
  

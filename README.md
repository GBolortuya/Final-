# Python - Max Heap Implementation and Application

# I. Introduction

As mentioned above  , the $\color{pale blue}{\textsf{PriorityQueue}}$  has some problems. The underlying principle of priority queue sorting is based on Max Heap. Let's take a look at the basic implementation and usage of Max Heap . First, let's clarify the concepts related to Max Heap and its implementation:

A. A maximum heap, also known as a large root heap (large top heap), means that the value of the root node (also called the top of the heap) is the largest value among all the nodes in the heap.

(1) The value of each root node $\color{red}{\textsf{is greater}}$  than that of its leaf nodes

(2) A maximum heap is a $\color{red}{\textsf{complete binary tree }}$ 

B. Complete binary tree, a binary tree with a depth of k and a number of nodes of 2^k - 1 is a complete binary tree

(1) Find the parent node given an index

![image](https://github.com/user-attachments/assets/d8dd4d41-0b1b-44bf-a45d-8f77166f7fcf)


(2) Find child nodes given an index

![image](https://github.com/user-attachments/assets/ed0f1f33-46d1-4df4-a8a2-92b60368570a)


# 2.Maximum heap implementation
  
# 1. Initialization
      
 (1) maxSize is the initialization array length of the maximum heap

 (2) count is the number of elements in the current maximum heap
    
 (3) The show function returns the current array

 ![image](https://github.com/user-attachments/assets/b5ed8cbb-84a6-4e7a-8e12-c8cda592e783)


# 2. Add elements 

(1) Add the node to the last position of the tree. The corresponding operation is to dispose the array count to the new value and count +1

(2) shift_up first finds the parent node of the current node. If it is smaller than the parent node, it exits directly. If it is larger than the parent node, it swaps positions with the parent node and recursively calls shift_up to continue searching upward until it is smaller than the parent node, then exits the loop.[9, 6, 5, 3, 1] => [9, 6, 7, 3, 1, 5]

![image](https://github.com/user-attachments/assets/31dd1351-0027-4d43-81b9-8bb36cf7b266)


![image](https://github.com/user-attachments/assets/4cbe9a5f-a3ba-4933-a617-7cc84f744544)


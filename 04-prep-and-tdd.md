## Big O: Analysis of Algorithm Efficiency
Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:

* Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

* Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions.


there is 4 Key Areas for analysis:
* Input Size(n to refer to the Input Size value.)
* Units of Measurement
* Orders of Growth
* Best Case, Worst Case, and Average Case

In order to quantify the Running Time in our analysis, we will consider Three Measurements of time:
* The time in milliseconds from the start of a function execution until it ends.
* The number of operations that are executed.
* The number of “Basic Operations” that are executed.

In order to quantify Memory Space, we can consider Four Sources of Memory Usage during function run-time:
* The amount of space needed to hold the code for the algorithm.
* The amount of space needed to hold the input data.
* The amount of space needed for the output data.


## Linked Lists
### What is a Linked List
A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

There are two types of Linked List - Singly and Doubly.

Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.


--a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.

---linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.
---In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

[Home](./README.md)<br>
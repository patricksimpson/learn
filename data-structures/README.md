## Data Structures

Based on the book: http://file.allitebooks.com/20190124/JavaScript%20Data%20Structures%20and%20Algorithms.pdf

### Sets
 * A *Set* is a group of definite, distinct objects. In layman’s terms, in programming, a set is a group of unordered unique (no duplicate) elements.
 Example, a set of integers may be {1, 2, 3, 4}. Within this, its subsets are {}, {1}, {2}, {3}, {4}, {1, 2}, {1, 3}, {1, 4}, {2, 3}, {2, 4}, {3, 4}, {1, 2, 3}, {1, 2, 4}, {1, 3, 4}, and {2, 3, 4 }.

 * Time Complexity:
   * Access: `O(1)`
   * Search: `O(1)`
   * Insert: `O(1)`
   * Remove: `O(1)`

### Hash Table

"A hash table is a fixed-sized data structure in which the size is defined at the start. This chapter explains how hash tables work by focusing on hashing, the method of generating a unique key. By the end of this chapter, you will understand various hashing techniques and know how to implement a hash table from scratch." (JavaScript Data Structures and Algorithms)

`localStorage` is an example of a hash table.

<img src="https://files.slack.com/files-pri/T024QRKC5-FG9FTSQN4/image.png">

### Hashing
* *Hashing* is used to map data of an arbitrary size to data of a fixed size. The values returned by a hash
  function are called hash values, hash codes, or simply hashes. If two keys map to the same value, a collision occurs
* **Hash Map**: a *hash map* is a structure that can map keys to values. A hash map uses a hash function to compute
  an index into an array of buckets or slots, from which the desired value can be found.
* Collision Resolution
 * **Separate Chaining**: in *separate chaining*, each bucket is independent, and contains a list of entries for each index. The
 time for hash map operations is the time to find the bucket (constant time), plus the time to iterate through the list
 * **Open Addressing**: in *open addressing*, when a new entry is inserted, the buckets are examined, starting with the
 hashed-to-slot and proceeding in some sequence, until an unoccupied slot is found. The name open addressing refers to
 the fact that the location of an item is not always determined by its hash value

### Stack
 * A *Stack* is a collection of elements, with two principle operations: *push*, which adds to the collection, and
   *pop*, which removes the most recently added element
 * **Last in, first out data structure (LIFO)**: the most recently added object is the first to be removed
 * Time Complexity:
   * Access: `O(n)`
   * Search: `O(n)`
   * Insert: `O(1)`
   * Remove: `O(1)`

JavaScript arrays implement stack-like properties.

### Queue
 * A *Queue* is a collection of elements, supporting two principle operations: *enqueue*, which inserts an element
   into the queue, and *dequeue*, which removes an element from the queue
 * **First in, first out data structure (FIFO)**: the oldest added object is the first to be removed
 * Time Complexity:
   * Access: `O(n)`
   * Search: `O(n)`
   * Insert: `O(1)`
   * Remove: `O(1)`

https://www.geeksforgeeks.org/implementation-queue-javascript/

<img src="https://www.thecrazyprogrammer.com/public_html/thecrazyprogrammer.com/wp-content/uploads/2016/05/Difference-Between-Stack-and-Queue.jpg">


### Linked List
 * A *Linked List* is a linear collection of data elements, called nodes, each
   pointing to the next node by means of a pointer. It is a data structure
   consisting of a group of nodes which together represent a sequence.
 * **Singly-linked list**: linked list in which each node points to the next node and the last node points to null
 * **Doubly-linked list**: linked list in which each node has two pointers, p and n, such that p points to the previous node and n points to the next node; the last node's n pointer points to null
 * **Circular-linked list**: linked list in which each node points to the next node and the last node points back to the first node
 * Time Complexity:
   * Access: `O(n)`
   * Search: `O(n)`
   * Insert: `O(1)`
   * Remove: `O(1)`

<img src="https://cdn-images-1.medium.com/max/1600/1*LCvUw4JaCiovZWeXb5zrMw.jpeg">

https://codeburst.io/js-data-structures-linked-list-3ed4d63e6571


### Heap
* A *Heap* is a specialized tree based structure data structure that satisfies the *heap* property: if A is a parent node of
B, then the key (the value) of node A is ordered with respect to the key of node B with the same ordering applying across the entire heap.
A heap can be classified further as either a "max heap" or a "min heap". In a max heap, the keys of parent nodes are always greater
than or equal to those of the children and the highest key is in the root node. In a min heap, the keys of parent nodes are less than
or equal to those of the children and the lowest key is in the root node
* Time Complexity:
  * Access Max / Min: `O(1)`
  * Insert: `O(log(n))`
  * Remove Max / Min: `O(log(n))`
  
  <img src="http://www.expertsmind.com/CMSImages/666_Heap%20Sort4.png">

https://codeburst.io/implementing-a-complete-binary-heap-in-javascript-the-priority-queue-7d85bd256ecf

### Graph
* A *Graph* is an ordered pair of G = (V, E) comprising a set V of vertices or nodes together with a set E of edges or arcs,
  which are 2-element subsets of V (i.e. an edge is associated with two vertices, and that association takes the form of the
  unordered pair comprising those two vertices)
 * **Undirected Graph**: a graph in which the adjacency relation is symmetric. So if there exists an edge from node u to node
 v (u -> v), then it is also the case that there exists an edge from node v to node u (v -> u)
 * **Directed Graph**: a graph in which the adjacency relation is not symmetric. So if there exists an edge from node u to node v
 (u -> v), this does *not* imply that there exists an edge from node v to node u (v -> u)

 https://www.geeksforgeeks.org/implementation-graph-javascript/


### Tree
 * A *Tree* is an undirected, connected, acyclic graph

### Binary Tree
 * A *Binary Tree* is a tree data structure in which each node has at most two children, which are referred to as
   the *left child* and *right child*
 * **Full Tree**: a tree in which every node has either 0 or 2 children
 * **Perfect Binary Tree**: a binary tree in which all interior nodes have two children and all leave have the same depth
 * **Complete Tree**: a binary tree in which every level *except possibly the last* is full and all nodes in the last
   level are as far left as possible

<img src="https://www.geeksforgeeks.org/wp-content/uploads/binary-tree-to-DLL.png">

  https://www.geeksforgeeks.org/implementation-binary-search-tree-javascript/

### Binary Search Tree
 * A binary search tree, sometimes called BST, is a type of binary tree which maintains the property that the value in each
   node must be greater than or equal to any value stored in the left sub-tree, and less than or equal to any value stored
   in the right sub-tree
 * Time Complexity:
   * Access: `O(log(n))`
   * Search: `O(log(n))`
   * Insert: `O(log(n))`
   * Remove: `O(log(n))`

https://khan4019.github.io/front-end-Interview-Questions/bst.html

### Trie
* A trie, sometimes called a radix or prefix tree, is a kind of search tree that is used to store a dynamic set or associative
  array where the keys are usually Strings. No node in the tree stores the key associated with that node; instead, its position
  in the tree defines the key with which it is associated. All the descendants of a node have a common prefix of the String associated
  with that node, and the root is associated with the empty String.

  https://youtu.be/7XmS8McW_1U

### Fenwick Tree
* A Fenwick tree, sometimes called a binary indexed tree, is a tree in concept, but in practice is implemented as an implicit data
  structure using an array. Given an index in the array representing a vertex, the index of a vertex's parent or child is calculated
  through bitwise operations on the binary representation of its index. Each element of the array contains the pre-calculated sum of
  a range of values, and by combining that sum with additional ranges encountered during an upward traversal to the root, the prefix
  sum is calculated
* Time Complexity:
  * Range Sum: `O(log(n))`
  * Update: `O(log(n))`

### Segment Tree
* A Segment tree, is a tree data structure for storing intervals, or segments. It allows querying which of the stored segments contain
  a given point
* Time Complexity:
  * Range Query: `O(log(n))`
  * Update: `O(log(n))`

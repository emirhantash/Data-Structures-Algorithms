# **Project 3**

## ***Binary Search Tree Project***
In computer science, a binary search tree (BST), also called an ordered or sorted binary tree, is a rooted binary tree data structure with the key of each internal node being greater than all the keys in the respective node's left subtree and less than the ones in its right subtree. The time complexity of operations on the binary search tree is directly proportional to the height of the tree.

Binary search trees allow binary search for fast lookup, addition, and removal of data items. Since the nodes in a BST are laid out so that each comparison skips about half of the remaining tree, the lookup performance is proportional to that of binary logarithm. BSTs were devised in the 1960s for the problem of efficient storage of labeled data and are attributed to Conway Berners-Lee and David Wheeler.

The performance of a binary search tree is dependent on the order of insertion of the nodes into the tree since arbitrary insertions may lead to degeneracy; several variations of the binary search tree can be built with guaranteed worst-case performance. The basic operations include: search, traversal, insert and delete. BSTs with guaranteed worst-case complexities perform better than an unsorted array, which would require linear search time.

The complexity analysis of BST shows that, on average, the insert, delete and search takes {\displaystyle O(\log n)}O(\log n) for {\displaystyle n}n nodes. In the worst case, they degrade to that of a singly linked list: {\displaystyle O(n)}O(n). To address the boundless increase of the tree height with arbitrary insertions and deletions, self-balancing variants of BSTs are introduced to bound the worst lookup complexity to that of the binary logarithm. AVL trees were the first self-balancing binary search trees, invented in 1962 by Georgy Adelson-Velsky and Evgenii Landis.

Binary search trees can be used to implement abstract data types such as dynamic sets, lookup tables and priority queues, and used in sorting algorithms such as tree sort.

![Binary Search Tree PNG](https://upload.wikimedia.org/wikipedia/commons/thumb/d/da/Binary_search_tree.svg/500px-Binary_search_tree.svg.png)
---
```
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] Write the Binary-Search-Tree stages of the sequence
```
* add 7
   ```
   7
   ```
* add 5
   ```
   5
    \
     7
   ```
* add 1
   ```
     5
    / \
   1   7
   ```
* add 8
   ```
     5
    / \
   1   7
        \
         8
   ```
* add 3
   ```
     5
    / \
   1   7
    \   \
     3   8
   ```
* add 6
   ```
      5
    /   \
   1     7
    \   / \
     3 6   8
   ```
* add 0
   ```
        5
      /   \
     1     7
    / \   / \
   0   3 6   8
   ```
* add 9
   ```
        5
      /   \
     1     7
    / \   / \
   0   3 6   8
              \
               9
   ```
* add 4
   ```
         5
      /     \
     1       7
    / \     / \
   0   3   6   8
        \       \
         4       9
   ```
* add 2
   ```
         5
      /     \
     1       7
    / \     / \
   0   3   6   8
      / \       \
     2   4       9
   ```



## ***Patika***
[patika.dev](www.patika.dev) 
## ***License***
[MIT](https://choosealicense.com/licenses/mit/)
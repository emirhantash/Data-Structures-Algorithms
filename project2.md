# **Project 2**

## ***Merge Sort Project***
Conceptually, a merge sort works as follows:

1. Divide the unsorted list into n sublists, each containing one element (a list of one element is considered sorted).
2. Repeatedly merge sublists to produce new sorted sublists until there is only one sublist remaining. This will be the sorted list.

![Merge Sort Example PNG](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Merge_sort_algorithm_diagram.svg/300px-Merge_sort_algorithm_diagram.svg.png) ![Merge Sort Animated GIF](https://upload.wikimedia.org/wikipedia/commons/thumb/c/cc/Merge-sort-example-300px.gif/220px-Merge-sort-example-300px.gif)

```
[16,21,11,8,12,22] -> Merge Sort
```
* **1. Problem**
    
    *Write the stages of the above array according to the sort type.*
 ---
* **2. Problem**

    *Write the Big-O notation.*
---
* ***Solution of the first problem*** 
    
    At the beginning, we divide our array into two. We divide the divided arrays again. We continue the process until only one element remains.
    ||||||||||||||
    |:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
    |We rewrite the array by dividing it into two.||||16|21|11|8|12|22||||			
    |We divide the left and right arrays into two again.|||16|21|11|||12|22		
    |We divide once more until only one element remains.||16|21||11|||8||12||22|
    ||16||21||11|||8||12||22

    After the division is finished, we combine our single-element arrays by binary. We continue this process until we get a sorted array.

    ||||||||||||||
    |:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
    ||16||21||11|||8||12||22
    |We combine them in binary order to merge||16|21||11|||8||12|22
    |We combine them in binary order again.|||11|16|21|||8|12|22||
    |In the final combine we get our array.|||8|11|12|16|21|22|||
---
* ***Solution of the second problem***
    
    Since it is a recursive function, it always calls itself and divides the array into two. For the Merge operation of each split array, since the length of the array is n so it will be O(n*(logn)) --> O(6*(log6)).
---
## ***Patika***
[patika.dev](www.patika.dev) 
## ***License***
[MIT](https://choosealicense.com/licenses/mit/)
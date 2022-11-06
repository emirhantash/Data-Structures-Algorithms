# **Project 1**

## ***Insertion Sort Project***
Insertion sort iterates, consuming one input element each repetition, and grows a sorted output list. At each iteration, insertion sort removes one element from the input data, finds the location it belongs within the sorted list, and inserts it there. It repeats until no input elements remain.

Sorting is typically done in-place, by iterating up the array, growing the sorted list behind it. At each array-position, it checks the value there against the largest value in the sorted list (which happens to be next to it, in the previous array-position checked). If larger, it leaves the element in place and moves to the next. If smaller, it finds the correct position within the sorted list, shifts all the larger values up to make a space, and inserts into that correct position.

![Insertion Sort Graphical Animated GIF](https://upload.wikimedia.org/wikipedia/commons/4/42/Insertion_sort.gif) ![Insertion Sort Animated GIF](https://upload.wikimedia.org/wikipedia/commons/0/0f/Insertion-sort-example-300px.gif)
---
* **1. Problem** 
```
 [22,27,16,2,18,6] -> Insertion Sort
 ```
 1. *Write the stages of the above sequence according to the sort type.*
 2. *Write the Big-O notation.*
 3. *Show the Time Complexity: Worst case/Average case/Best case* 
 4. *After the array has been sorted, Which case is 18 has belong*
---
* **2. Problem**
```
[7,3,5,8,2,9,4,15,6] Write the first 4 steps of this array according to the Insertion Sort.
```
---
* ***Solution of first problem***
1. Step 1: Our first number (22) cannot be sorted by itself. Now the data looks like this:
   ```
    22 | 27 16 2 18 6
   ```

   Step 2: 22 and 27 datas are compares. Since 22 is more less than 27, the first two data are complete. No changes are made. Now the data looks like this:
   ```
    22 27 | 16 2 18 6
   ```

   Step 3: 22 27 sequential data is compares with 16. Since 16 is less than 22 and 27, it precedes the data and our data look like this:
   ```
    16 22 27 | 2 18 6
   ```
   Step 4: 16 22 27 sequential data is compares with 2. 2 will be the smallest number in the data. Therefore, it goes to the beginning of the data. Now our data looks like this:
   ```
    2 16 22 27 | 18 6 
   ```
   Step 5: 2 16 22 27 sequential data is compares with 18. 18 is greather than 2 and 16; less than 22 and therefore less than 27 either. 18 takes its place in the data. Now our data looks like this:
   ```
    2 16 18 22 27 | 6
   ```
   Step 6: 2 16 18 22 27 sequential data is compares with 6. 6 is greater than 2, less than 16 and therefore less then the rest of data either. 6 takes its place in the data. Now our data looks like this:
   ```
    2 6 16 18 22 27 |
   ```
   Step 7: Our data has been sorted now and looks like this:
   ```
    2 6 16 18 22 27
   ```
2. Big-O notation: O(n^2)
3. 
   * **Worst case:** The number we are looking for is at the end, Given the opposite array, then each element of the array will be smaller than the one after it. Therefore, the inner loop will move 0 for element 1, backward 1 for element 2, 2 for element 3, then 3 4 5 6… n. So 0+1+2+3+4…..+n-1 = [n*(n-1)]/2 : O(n^2)
   * **Average case:** The number we are looking for is in the middle, when we take the average of the worst case and the best case, we find it as O(n^2).
   * **Best case:** The number we're looking for is at the very beginning of the array. The full ordered sequence goes over n numbers once and stays with this one pass as there is no need to advance any of them backwards. So it would be O(n) or more correct to say O(1).
4. 18 is in the scope of the average case because it's in the middle of the data set.
---
* ***Solution of second problem***

   Step 1:
   ```
    7 | 3 5 8 2 9 4 15 6
   ```
   Step 2:
   ```
    3 7 | 5 8 2 9 4 15 6
   ```
   Step 3:
   ```
    3 5 7 | 8 2 9 4 15 6
   ```
   Step 4:
   ```
    3 5 7 8 |  2 9 4 15 6
   ```
---
## ***Patika***
[patika.dev](www.patika.dev) 
## ***License***
[MIT](https://choosealicense.com/licenses/mit/)
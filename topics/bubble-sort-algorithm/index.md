# Bubble sort algorithm

Bubble sort is a simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. The pass through the list is repeated until the list is sorted. It is named "bubble sort" because the smaller elements "bubble" to the top of the list as the algorithm progresses. 

Bubble sort is not efficient for large lists, but it is easy to understand and implement, making it a common educational example. 

Bubble sort can be optimized by adding a flag to check if any swaps were made during a pass. If no swaps are made in a pass, the list is already sorted, and the algorithm can terminate early.

Steps:

1. Start: Begin at the first element (index 0) of the list.

2. Compare Adjacent Elements: Compare the first element with the second element. If the first element is greater than the second, swap them.

3. Move to Next Pair: Move to the next pair of elements (the second and third, then the third and fourth, and so on) and repeat step 2.

4. Continue: Continue this process of comparing and swapping adjacent elements as you move through the list. After the first pass, the largest element is guaranteed to be at the end of the list.

5. Repeat: Repeat the process for a total of n-1 passes, where n is the number of elements in the list. After each pass, the largest unsorted element will "bubble up" to its correct position.

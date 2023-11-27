# Insertion sort algorithm

Insertion sort is a simple sorting algorithm that builds the final sorted array one item at a time. It works by taking one element from the unsorted part of the list and inserting it into its correct position in the sorted part of the list. Insertion sort is efficient for small lists or lists that are mostly sorted.

Insertion sort has a time complexity of O(n^2) in the worst and average cases, where "n" is the number of elements in the list. It performs well for small lists and is more efficient than other sorting algorithms like Bubble Sort for most real-world scenarios.

Steps:

1. Start: Begin with the second element (index 1) of the list. The first element is considered to be in the sorted part by itself.

2. Compare and Insert: Compare the current element with the previous elements in the sorted part of the list. Insert the current element into its correct position in the sorted part by shifting larger elements to the right.

3. Repeat: Continue this process for the remaining unsorted elements, one at a time, until the entire list is sorted.

4. End: The list is now sorted.


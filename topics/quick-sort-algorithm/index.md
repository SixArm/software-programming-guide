# Quick sort algorithm

Quick sort is a widely used, efficient, and in-place sorting algorithm. It is a divide-and-conquer algorithm that works by selecting a "pivot" element from the array and partitioning the other elements into two sub-arrays, according to whether they are less than or greater than the pivot. The sub-arrays are then sorted recursively. Quick sort is known for its speed and is commonly used in many programming libraries and applications.

Steps:

1. Choose a Pivot: Select a pivot element from the array. The choice of the pivot can be made in various ways, but typically it's the middle element.

2. Partitioning: Rearrange the elements in the array so that all elements less than the pivot come before it, and all elements greater than the pivot come after it. The pivot is now in its final sorted position.

3. Recursion: Apply the Quick sort algorithm recursively to the sub-array of elements less than the pivot and the sub-array of elements greater than the pivot.

4. Combine: The sorted sub-arrays are combined to produce the final sorted array.

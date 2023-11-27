# Merge sort algorithm
 
Merge sort is an efficient, comparison-based sorting algorithm that follows the divide-and-conquer strategy to sort a list or array. It works by dividing the unsorted list into smaller sublists, sorting each sublist, and then merging the sorted sublists back together to create a single sorted list. Merge sort is a stable sorting algorithm and is often used as a standard for sorting.

Merge sort has a time complexity of O(n log n) and is known for its stable and efficient sorting performance.

Steps…

Divide: Divide the unsorted list into two halves, roughly equal in size. If the list has an odd number of elements, one of the halves will have one more element than the other.

Conquer: Recursively sort each of the two sublists. This is done by applying the Merge sort algorithm to each sublist.

Merge: Combine the two sorted sublists from the conquer step to create a single sorted list. The merging process involves comparing elements from the two sublists and adding the smaller element to the new merged list. This continues until all elements from both sublists are included in the merged list.

Repeat: Continue dividing and merging until you have a single sorted list containing all elements from the original unsorted list.

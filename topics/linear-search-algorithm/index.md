# Linear search algorithm

A linear search algorithm, also known as a sequential search algorithm, is a straightforward method for finding a specific element within a list or array. It works by iterating through the elements one by one until the target element is found or until the entire list has been searched. 

Its time complexity is `O(n)`, where n is the number of elements in the list, which means the time it takes to complete the search increases linearly with the size of the list. For large datasets, more efficient search algorithms are used, such as binary search or hash tables.

Steps:

1. Start at the beginning of the list of elements.

2. Compare the target element you are searching for with the current element in the list.

3. If the current element matches the target element, the search is successful, and you can return the index of the current element (or any other relevant information).

4. If the current element does not match the target element, move to the next element in the list.

5. Repeat until you either find the target element or reach the end of the list without finding a match.

6. If you reach the end of the list without finding the target element, the search is unsuccessful, and you can return a specified value (e.g., -1) to indicate that the element was not found.

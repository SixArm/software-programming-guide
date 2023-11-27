# Search algorithms

Search algorithms are used to find an element with a specific property within a collection of data.

Some common ones:

* Linear search is the most basic search algorithm. It sequentially checks every element in the collection until the desired element is found or the end of the collection is reached.

* Binary search is applicable to sorted collections, and much more efficient than linear search. Binary search works by repeatedly dividing the collection in half until the desired element is found. At each step, the algorithm compares the target element to the middle element of the current range. If the target is smaller, the algorithm repeats the search on the left half of the range. If the target is larger, the algorithm repeats the search on the right half of the range.

* Interpolation search is similar to binary search, but it is more efficient for collections with uniformly distributed elements. Interpolation search works by using the value of the target element and the values of the first and last elements in the collection to estimate the position of the target element. The algorithm then narrows the search range based on this estimate and continues with a binary search.

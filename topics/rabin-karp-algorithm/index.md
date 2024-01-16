# Rabin-Karp algorithm

The Rabin-Karp algorithm is a string searching algorithm that efficiently finds all occurrences of a pattern string within a longer text string.

The algorithm creates a rolling hash function that hashes a window of characters in the text and compares the hash value of that window with the hash value of the pattern. The rolling hash function is crucial to the efficiency, and must be designed to quickly update the hash value when a new character enters the window or old character exits the window.

The Rabin-Karp algorithm has an average-case time complexity of `O(n+m)`. This makes it efficient for string searching, especially when the pattern is much shorter than the text. Worst-case behavior is if hash collisions occur frequently, leading to time complexity of `O(n*m)`.

Steps:

1. Calculate the hash value of the pattern string.

2. Initialize a sliding window of the same length as the pattern at the beginning of the text and calculate its hash value.

4. Iterate through the text from left to right, moving the sliding window one character at a time.

5. At each step, compare the hash value of the current window with the hash value of the pattern.

6. If the hash values match, perform a full string comparison to verify if it's a true match.

7. If they don't match, continue moving the window and recalculating the hash value.

8. Keep track of the positions where a match is found, and continue the process until the end of the text.

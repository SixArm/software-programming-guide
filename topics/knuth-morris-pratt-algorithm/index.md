# Knuth-Morris-Pratt algorithm

The Knuth-Morris-Pratt (KMP) algorithm is a string searching algorithm that efficiently finds occurrences of a pattern string within a longer text string. It is known for its linear time complexity, making it very efficient for searching in practice.

The KMP algorithm works by using a preprocessed "failure function" or "partial match table" to avoid unnecessary character comparisons when a mismatch occurs between the pattern and the text. Instead of starting the comparison from the beginning of the pattern for each mismatch, it jumps ahead based on information from the failure function.

The Knuth-Morris-Pratt algorithm has a time complexity of `O(n+m)`, where n is the length of the text and m is the length of the pattern, making it an efficient choice for string searching tasks.

Steps:

1. Pre-process: Construct a failure function that is used to determine how far to skip ahead in the text when a mismatch occurs between the pattern and the text. This function is often referred to as the "partial match table" or "failure table."

2. Search: Iterate through the text while comparing characters from the pattern and the text. When a mismatch occurs at position i in the pattern, use the value in the failure function (i.e., failure[i]) to determine how far to skip ahead in the text. Update the pointer in the pattern (i) accordingly and continue comparing characters.

3. Match: When a complete match is found (i.e., i reaches the end of the pattern), record the position in the text where the match starts.

4. Continue searching for additional occurrences of the pattern in the text.

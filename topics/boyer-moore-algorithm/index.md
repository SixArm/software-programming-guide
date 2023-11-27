# Boyer-Moore algorithm

The Boyer-Moore algorithm is an efficient string searching algorithm used to find occurrences of a pattern string within a longer text string. It is a preferred choice when searching for multiple occurrences of a pattern. Average-case time complexity is `O(n+m)`.

Two key strategies:

* Bad Character Rule: Focus on the last character of the pattern and determines how much to shift the pattern to align the mismatched character in the text with the last occurrence of that character in the pattern. If the mismatched character in the text does not appear in the pattern, the pattern can be shifted by the length of the pattern itself.

* Good Suffix Rule: Handle situations where a suffix of the pattern matches part of the text, but a mismatch occurs afterward. It looks for the longest suffix of the pattern that matches a substring to the left of the mismatched part. The pattern is then shifted so that the last occurrence of this matching suffix aligns with the mismatched portion of the text.

Steps:

1. Preprocesses the pattern to create two tables: a bad character table that stores the shift values for each character in the pattern, and a good suffix table that stores the shift values for the good suffixes of the pattern.

2. Initialize two pointers, `i` and `j`, to the end of the pattern and the end of the text, respectively.

3. Compare the characters at `i` (pattern) and `j` (text). If they match, decrement both `i` and `j`. If they don't match, use the bad character and good suffix rules to calculate the maximum shift amount and move j accordingly.

4. Repeat until a match is found or `j` goes beyond the end of the text.

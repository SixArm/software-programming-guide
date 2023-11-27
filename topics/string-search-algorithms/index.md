# String search algorithms

String search algorithms, also known as string matching algorithms, are used to find the occurrences of a substring (or pattern) within a larger string. Complexity is often notated by `m` as the length of the substring (or pattern), and `n` as the length of the larger string.

Some common ones:

* Brute Force (Naive) String Search: Check for a pattern match at each possible starting position. Time complexity `O(n*m)`.

* Knuth-Morris-Pratt (KMP) Algorithm: Preprocess the pattern to determine the maximum length of the proper suffix that matches a proper prefix. Use this data to avoid unnecessary comparisons during string searching. Time complexity `O(n+m)`.

* Boyer-Moore Algorithm: Use two heuristic rules, the bad character rule and the good suffix rule, to skip comparisons and achieve sublinear time complexity in practice.

* Rabin-Karp Algorithm: Use rolling hashes to compare substrings of the text with the pattern.

* Aho-Corasick Algorithm: Build a finite automaton that recognizes all the patterns and processes the text in a single pass. Good for multiple patterns.

* Z-Algorithm: Computes the Z-array, which represents the longest substring starting from each position that matches the beginning of the text. Good for multiple patterns.

* Trie Data Structure: A tree-like structure that stores a dynamic set of strings. It is useful for dictionary search and autocomplete.

* Regular Expressions (Regex): A powerful way to define search patterns for text using a formal language. Regex engines are available in many programming languages and are widely used.

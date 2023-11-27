# Bloom filter

A Bloom filter is a probabilistic data structure used to test the membership of an element in a set. It provides a way to quickly and efficiently determine whether an element is not in a set. It is named after Burton Bloom, who invented the concept in 1970.

A Bloom filter consists of a bit array of m bits and k hash functions. Initially, all bits are set to 0. When an element is added to the set, it is hashed by the k hash functions, and the resulting k hash values are used to set the corresponding bits in the bit array to 1. To check whether an element is in the set, the element is hashed by the same k hash functions, and the corresponding bits in the bit array are checked. If any of the bits are 0, the element is definitely not in the set. If all the bits are 1, the element is probably in the set.

The probability of a false positive (i.e., the Bloom filter reporting that an element is in the set when it is not) can be adjusted by choosing the size of the bit array and the number of hash functions. A larger bit array and more hash functions will reduce the probability of false positives, but will also increase the memory usage and computational overhead of the Bloom filter.

Bloom filters have many applications in computer science, such as in web caching, spell checking, network routers, and DNA sequence analysis. They are particularly useful in situations where the size of the set is large and it is not feasible to store all the elements, or where the cost of false positives is low compared to the cost of false negatives.
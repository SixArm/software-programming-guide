# Hash table (a.k.a. hash map)

A hash table, also known as a hash map, is a data structure that provides efficient data retrieval by using a key to access a value. It is based on the concept of hashing, which involves converting the key into an index within an array or hash table, allowing for quick lookups and insertions. Hash tables are widely used in computer science and are the basis for various associative array data structures like dictionaries and sets.

Key aspects…

Hash Function: A hash function takes a key as input and generates an index within the hash table. The quality of the hash function directly impacts the performance of the hash table. A good hash function should distribute keys uniformly across the available hash table slots.

Array or Bucket: The hash table itself is usually an array of fixed or dynamic size, called buckets or slots. Each slot can store one or more key-value pairs. The size of the array influences the efficiency of the hash table.

Retrieve: To retrieve a value associated with a given key, the same hash function is applied to the key to find the corresponding index in the hash table. The value at that index is returned. If chaining is used, the elements in the bucket may need to be searched linearly.

Insert: To insert a key-value pair into the hash table, the hash function is applied to the key to determine the index in the array where the pair should be stored. If multiple pairs map to the same index (a collision), various collision resolution techniques can be used, such as chaining (using linked lists) or open addressing.

Delete: To delete a key-value pair, the key is hashed to determine the index and then removed from the array. Handling collisions during deletion depends on the collision resolution technique used.

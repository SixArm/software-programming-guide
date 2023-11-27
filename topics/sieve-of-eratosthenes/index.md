# Sieve of Eratosthenes

The Sieve of Eratosthenes is an algorithm for finding all the prime numbers up to a given limit. It is named after the ancient Greek mathematician Eratosthenes who first described the algorithm.

The algorithm works by marking all the multiples of each prime number, starting with 2, and eliminating the composites. The remaining numbers that are not marked are prime.

Steps:

1. Create a list of integers from 2 to the given limit.

2. Start with the first prime number, which is 2.

3. Mark all the multiples of 2 in the list as composite (not prime).

4. Find the next prime number, which is the smallest number in the list that is not yet marked as composite.

5. Repeat steps 3 and 4 until you have checked all the numbers up to the square root of the given limit.

6. The remaining numbers in the list that are not marked as composite are prime.

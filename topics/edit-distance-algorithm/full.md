# Edit distance algorithm

The Edit Distance (also known as Levenshtein Distance) is a measure of the similarity between two strings. It quantifies the minimum number of single-character edits (insertions, deletions, or substitutions) required to change one string into the other. The Edit Distance algorithm has applications in various fields, including natural language processing, DNA sequence alignment, and spell checking.

Here's a dynamic programming-based approach to compute the Edit Distance between two strings…

1. Initialization: Create a matrix (2D array) with dimensions (m+1) x (n+1), where "m" is the length of the first string, and "n" is the length of the second string. Initialize the first row and the first column of the matrix with values from 0 to m and 0 to n, respectively, representing the cost of converting an empty string to a string of length "i" (for the first row) or converting a string of length "j" to an empty string (for the first column).

2. Filling the Matrix: Iterate over each cell in the matrix, starting from cell (1,1) up to cell (m,n). 

3. For each cell (i, j), calculate the minimum of the following three values: the value in the cell to the left (representing deletion), the value in the cell above (representing insertion), and the value in the cell diagonally above and to the left (representing substitution). 

4. Add 1 to the minimum value if the characters in the two strings at positions i-1 and j-1 are not the same (indicating a substitution is needed).

5. Result: The value in the cell at the bottom right corner (cell m, n) represents the minimum edit distance between the two strings.

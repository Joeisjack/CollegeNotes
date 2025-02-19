```cpp 
int min;
for(int i = 0; i < n - 1); i++{
	min = i;
	
	for(int j = i + 1; j < n; j++){
		if(A[j] < A[min]){
			min = j;
		}
	}
	
	swap(A[i], A[min]);
}
```
Something about proving this code is $n^2$
$\sum_{i=0}^{n-2}\sum_{i+1}^{n-1}1=\sum_{i=0}^{n-2}\left(n-1-\left(i+1\right)+1\right)=\sum_{i=0}^{n-2}\left(n-i-1\right)$

Brute-Force String Matching
	Pattern: A string of m characters to search for
	Text: A (longer) string of n chars to search in
	Problem: Find a substring in the text that matches
The Algorithm:
	Step 1:
		Align pattern at the beginning of text
	Step 2:
		Moving from left to right, compare each char of pattern to the corresponding character in text until...
			All characters are found to match; or
			A mismatch is detected
	Step 3:
		While the pattern is not found and the text is not exhausted, realign pattern one position to the right and repeat Step 2

Hamiltonian Cycle:
	Visits every vertex exactly once and comes back to its starting vertex
	There are exactly $\left(n-1\right)!$ Possibilities (AKA permutations)
Euler Cycle:
	Visits every edge exactly once and comes back to its starting vertex



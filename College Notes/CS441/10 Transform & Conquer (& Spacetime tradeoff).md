Remember: 
Comparison based sorting cannot get faster than O(n log n) time

## Instance Simplification
Given: A system of n linear equations in n unknowns with an arbitrary coefficient matrix
Transform to: An equivalent system of n linear equations in n unknowns with an upper triangular coefficient matrix

Steps (Back substitution)
1. Put into form of a matrix
	$\begin{matrix} 2x_1 - 4x_2 + x_3 = 6 \\ 3x_1 - x_2 + x_3 = 11 \\ x_1 - x_2 + x_3 = -3 \end{matrix}$
	INTO:
	$\begin{matrix} 2 & -4 & 1 & 6 \\ 3 & -1 & 1 & 11 \\ 1 & -1 & 1 & -3 \end{matrix}$
2. Triangularize (Make the first time a x appears the only time)
	$\begin{matrix} 2 & -4 & 1 & 6 \\ 0 & 5 & -\frac12 & 1 \\ 0 & 0 & -\frac65 & -\frac{36}5 \end{matrix}$
	You can figure out how this happens

Know Heaps and Heap sort

```psudo
// Input: An array A[0, n-1]
// Output: Array S[0, n-1] of A's elements in non decreasing order

for(i = 0; i < n; i++){
	Count[i] = 0;
}
for(i = 0; i < n; i++){
	for(j = i + 1; j < n; j++){
		if(A[i] < A[j]){
			Count[j]++;
		}
		else{
			Count[i]++;
		}
	}
}
for(i = 0; i < n; i++){
	S[Count[i]] = A[i];
}
```

Time Complexity: O($n^2$)
Space Complexity: O($n$)



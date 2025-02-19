Induction:
P(n): 1 + 2 + ... + n = (n * (n - 1)) / 2
P(1): Basis Step
P(k) => P(k+1): Inductive step

EXAMPLE:
Loop Invariant
```cpp
for(i = 0; i < n; i++){

}
```

Property === Invariant
P(0):
	i == j   =>   i == j + 1 property will again hold

[[Loop Invariant Example]]

Selection Sort Pseudo Code
```psudo
	sort(int A[])
		for(all numbers except things already sorted)
			Find lowest number
			Swap with lowest index unsorted number
		return A[]
```

Actual
```cpp
	for(int i = 0; i < n - 1; i++){
		int min = i;
		for(int j = i + 1; j < n; j++){
			if A[j] < A[min];
			min = j;
		}
		swap(A[i], A[min]);
	}
```
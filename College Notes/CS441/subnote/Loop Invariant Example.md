Searching

```cpp
int searchArray(int A[], int n, int key){
	int i = 0;
	while(i <= n && A[i] != key){
		i++;
	}
	
	if(i < n){
		return i
	}
	else{
		return -1
	}
}
```

Loop Invariant:
	After the iteration i == j

A1(j): j < n
A2(j): ForAll 0 <= k <= j;  A\[k] != key

Initialization:
	d
Maintinence:
	Assume A1(j) is true
	A2(j) is true

The possibilities:
	When i == j+1
		case 1: A\[j + 1] != key
			AND   ForAll 0 <= k <= j + 1     A\[k] != key
			=> ForAll 0 <= k <= j +1      A\[k] != key
			Ergo   A2(j + 1) is true
		case 2: A\[j + 1] == key
			AND   0 <= k <= j     A\[k] != key
			A\[j + 1] is the first occurrence of key and the algorithm correctly returns j + 1
		case 3: j + 1 == n
			Ergo A2\(n - 1) is true by the inductive hypothesis/maintenance condition
			=> ForAll 0 <= k <= n - 1     A\[k] != key
			So key is not in the array
			Algorithm correctly returns -1




PART 2:

```cpp
int maxValArray(int A[], int n){
	int maxVal = A[0];
	for(int i = 1; i < n; i++){
		if(A[i] > maxVal){
		maxVal = A[i];
		}	
	}
	return maxVal;
}
```

Loop Invariant:

A1(j): j < n
A2(j): ForAll 0 <= k <= j;  A\[k] != maxVal
A3(j): There exists L such that 0 <= L <= j && A\[L] == maxVal

Maintenance:
	Assume
		A1(j) is true
		A2(j) is true
		A3(j) is true
	for some j

When i == j + 1 finishes:
	case 1: Suppose A\[j + 1] > maxVal
		ergo maxVal will now be equal to A\[j + 1]
		A3\[j + 1] is true
		Also A2(j) && (A\[j + 1] > maxVal) => A2\[j + 1]
	case 2: Suppose A\[j + 1] < maxVal
		So the value of maxVal does not change
		A2(j) && (A\[j + 1] < maxVal) => A2\[j + 1]
		A3\[j] =? A3\[j + 1]

Termination:
Case 3:
	j + 1 == n
	ergo A2(n - 1) is true AND A3(n - 1) is true
	ergo The algorithm correctly returns the maxVal


Gaussian Elimination
	https://en.wikipedia.org/wiki/Gaussian_elimination
	Yeah, deal with it future me

Matrix Addition
	(n * n matrix) + (n * n matrix) = (n * n matrix)
	You literally just add every element with the corresponding element in other matrix

Matrix Multiplication
	Cols should be the same as Rows on the other matrix
	You end up with a n * n matrix
![[Matrix Multiplication.png]]
	Where Matrix A is multiplied with Matrix B
	Has a time complexity of n^3 (3 for loops, all nested)

An integer n requires (log_2 n) bits to store n

Algorithm to count the number of bits in integer n
```python
count = 1
while n > 1 do
	count++
	n /= 2

return count
```

Steps for analysis of recursive algorithms
	Decide on a parameter for input size
	Identify the basic operations
	Will the number of basic operations change based on input size?
	Set up a recurrence growth
	???
	Profit

[[Recursive Analysis of n!]]

[[Tower of Hanoi Puzzle]]

The time complexity is not the actual amount of time to do a task
It's actually the amount of "moves" that an algorithm does (Think Tower of Hanoi)
Think of the number of basic actions


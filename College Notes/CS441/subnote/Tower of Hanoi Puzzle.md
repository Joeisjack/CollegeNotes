![[Tower of Hanoi Drawing.png]]

n = number of disks

n = 2 ---> 3 moves
	a -> b
	a -> c
	b -> c

n = 3 ---> 7 moves
	a -> c
	a -> b
	c -> b
	a -> c
	b -> a
	b -> c
	a -> c

Recursive Analysis
	M(n) = number of disk moves to move n disks from tower 1 to tower 3
	M(n) = 2 * M(n - 1) + 1, T(1) = 1
	That's the time complexity
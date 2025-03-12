Divide the instance of the problem into two or more smaller instances

Usually recursive

Merging two arrays b, c into one array a
```psudo
for every i item in b
	a[i] = b[i]

for every i item in c
	a[i + b.len] = c[i]
```


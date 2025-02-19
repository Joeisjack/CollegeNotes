T(n) = 1 + T(n - 1) for all n >= 1, T(0) = 1

T(n - 1) = 1 + T(n - 2) for all n >= 2

Substitute

T(n) = 1 + 1 + T(n - 2) for all n >= 2

...

T(n) = i + T(n - i)

The algorithm will terminate when (i == n)

Time complexity is
(n + 1) = Theta(n)


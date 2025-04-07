There are two kinds of uncertainty.
One where you don't know the outcome before it happens (pre-coinflip)
The other where you don't know the outcome after it happens (hidden result)

[Bayesian Probability](https://en.wikipedia.org/wiki/Bayesian_probability)

$P$ represents a pure state if and only if $P^2=P$ and if and only if $Tr\left(P^2\right)=1$

## Properties of Density Operators
1. $P$ is Hermitian, i.e., $P^{\dagger}=P$
2. $Tr\left(P\right)=1$
3. $P$ is positive semi-definite
	Above means all eigenvalues are $\ge0$

## Basis
1. Standard Computational
	$\ket0,\ket1$
2. x-Basis or $\pm$-Basis
	$\ket+, \ket-$
3. y-Basis or $\pm i$-Basis
	$\ket i, \ket {-i}$


For the following mixed ensemble:

$\begin{matrix} \ket+ & \ket{i} & \ket1 \\ 1/4 & 1/4 & 1/2 \end{matrix}$

$P = 1/4 \ket+ \bra+ + 1/4 \ket{i} \bra{i} + 1/2 \ket1 \bra1$
$\frac{1}{4} \frac1{\sqrt2} \begin{pmatrix} 1 \\ 1 \end{pmatrix} \frac1{\sqrt2} (1, 1) + \frac14 \frac1{\sqrt2} \begin{pmatrix} 1 \\ i \end{pmatrix} \frac1{\sqrt2} (1, -i) + \frac12 \begin{pmatrix} 0 \\ 1 \end{pmatrix} (0, 1)$
$\frac18 \begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix} + \frac18 \begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix} + \frac12 \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} \frac14 & \frac{1-i}{8} \\ \frac{1+i}8 & \frac34 \end{pmatrix}$

A good exam question would be on mixed ensembles and doing what above

# Bloch Sphere

$S^0$ = Two Points
$S^1$ = Circle
$S^2$ = Surface of a Ball
$S^3$ = 3-Sphere (point at infinity)

The sphere encloses a big "hole". It's hollow

$f:\left\lbrace0,1\right\rbrace^{n}\to\left\lbrace0,1\right\rbrace^{m}$
 Objective: Compile into unitary op $U_{f}$
 Problem: F may not be bijective i.e, reversible but $U_{f}$ is reversible

$\begin{matrix} f \\ x \to y \\ x \to f(x) \end{matrix}$

$x\cdot y\to x\cdot y$
$\left(x,y\right)\to\left(f\left(x\right)+y\right)$

$\left(x,y\right)\to\left(x,f\left(x\right)+y\right)\to\left(x,f\left(x\right)+\left(f\left(x\right)+y\right)\right)_{}=\left(x,y\right)$

[[Gates]]
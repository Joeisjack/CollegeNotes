A 1D complex line is a 2D real plane

The orthonormal (perpendicular and all unit length (normalized :D)) basis is known as the computational basis or standard basis.
ex:
$\ket0,\ket1$

With the computational basis, any element in the space can be made with a linear combination of those vectors
ex:
$\ket\psi = a\ket0 + b\ket1$

Tensor Product
$A \otimes B$
$\begin{pmatrix} a_{00} & a_{01} \\ a_{10} & a_{11} \end{pmatrix} \otimes \begin{pmatrix} b_{00} & b_{01} \\ b_{10} & b_{11} \end{pmatrix} = \begin{pmatrix} a_{00}b & a_{01}b \\ a_{10}b & a_{11}b \end{pmatrix}$
This will result in a 4 * 4 matrix

Remember binary numbers can be represented as kets
$5 = 101 \rightarrow \ket1 \otimes \ket0 \otimes \ket1$
Creates a 1 * 8 matrix! This gets very large

$\ket0\bra1$ and $\bra{1}{0}\rangle$ are VERY different
The first is an outer product and the second is just a scalar

$\ket\psi = a\ket0 + b\ket1 =\bra0\psi\rangle\ket0 + \bra1\psi\rangle\ket1 = \ket0\bra0\psi\rangle + \ket1\bra1\psi\rangle = (\ket0\bra0 + \ket1\bra1)\ket\psi$

$\ket0\bra0 + \ket1\bra1 = I$ or the Identity matrix! :O

$\bra0\psi\rangle = \bra0a\ket0 + \bra0b\ket1$

Quantum Computing Instructions
U -> Unitary ops
$\Omega$ -> Hermition ops
x, y, z -> Pauli spin ops
$\begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix}, \begin{pmatrix}0 & i \\ -i & 0 \end{pmatrix}, \begin{pmatrix}1 & 0 \\ 0 & -1 \end{pmatrix}$

[[Gates]]

Measurement Level 1:
$\ket\psi = a\ket0 + b\ket1 \rightarrow$ measured w.r.t $\ket0, \ket1$ -> $P_0 = \left|a\right|^2$ and $P_1=\left|b\right|^2$

Lets take a qubit
$\ket\psi = a\ket0 + b\ket1 \approx \ket0 + (b / a)$
Multiply by $a^{-1}$
$\ket1 = 0\ket0 + \ket1$     $b/a = \infty$ 

H which is in the $C^2$ space -> Complex Plane in the $C$ space

$\approx \ket0 + (b/a)\ket1 \approx b/a = e+it$

Adding the point of infinity to a plane creates the shape of a sphere

The state space of a sphere $= S^2$ aka the Bloch Sphere

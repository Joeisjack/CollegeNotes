Let there be a 2D Hilbert Space H
$\ket\psi = z_0\ket0 + z_1\ket1$
$=(x_0+iy_0)\ket0 + (x_1+iy_1)\ket1$

$Dim_CH = 2$
$Dim_RH = 4$

$= x_0 \ket0 + y_0 (i \ket0) + x_1 \ket1 + y_1 (i \ket1)$

Real Basis
$\ket0, i\ket0, \ket1, i\ket1$

Complex Basis
$\ket0, \ket1$
H -> C

$\ket\psi = a\ket0 + b\ket1 \rightarrow \frac ab \text{ if b} \neq 0$

$\approx\frac ab\ket0 + \ket1 \rightarrow \infty \text{  if b}=0$

## Reverse Stereographic Projection

![[Reverse Stereo Projection.png]]

Is point on the Bloch sphere.

Quirk/Wong convention WILL be used in quiz

Remember Pauli Gates
[[Gates]]

## The Three Orthonormal Basis
$\ket0$
$\ket1$
$\ket{+} = \frac {\ket0 + \ket1}{\sqrt 2}$ 
$\ket{-} = \frac {\ket0 - \ket1} {\sqrt2}$
$\ket i = \frac {\ket0 + i\ket1}{\sqrt2}$
$\ket {-i} = \frac {\ket0 - i\ket1}{\sqrt2}$

## Orthogonal Projectors
$P_0=\ket0\bra0$
$P_1=\ket1\bra1$
$P_+ = \ket + \bra +$
$P_- = \ket - \bra -$
$P_i = \ket i \bra i$
$P_{-i} = \ket {-i} \bra {-i}$

Complete Collection of Orthogonal Projectors

__Complete__ means $P_++P_- = 1$
$P^2 = p$
Projector Idempotent



Measure $\ket\psi$ with respect to orthonormal basis $\ket0, \ket1$
$\ket\psi = a\ket0 + b\ket1$

$P_0 = \text {prob}(\ket0) =|a|^2$
$P_1 = \text {prob}(\ket1) =|b|^2$

normalized means $|a|^2 + |b|^2 = 1$

How about...
Measure $\ket\psi$ with respect to orthonormal basis $\ket+, \ket-$
$\ket\psi = \alpha\ket+ + \beta\ket-$
$\ket\psi = 1\ket\psi = P_+\ket\psi + P_- \ket\psi$
$=\ket+\bra+\psi\rangle + \ket-\bra-\psi\rangle$
$= \bra+\psi\rangle \ket+ + \bra-\psi\rangle \ket-$

$P_+ = \text {prob}(\ket+) =|a|^2 = |\bra+\psi\rangle|^2$
$P_- = \text {prob}(\ket-) =|b|^2 = |\bra-\psi\rangle|^2$

Exam Stuff!!!
Bell States

## Bell Basis

$\frac {\ket {00} + \ket {11}} {\sqrt2}$
$\frac {\ket {00} - \ket {11}} {\sqrt2}$
$\frac {\ket {01} - \ket {10}} {\sqrt2}$
$\frac {\ket {01} + \ket {10}} {\sqrt2}$

->
We kinda assume that it is entangled
$\frac {\ket0\ket0 + \ket1\ket1}{\sqrt2} = (\frac {a\ket0 + b\ket1}{\sqrt2})(\frac {c\ket0 + d\ket1}{\sqrt2})$
$= \frac 12 (ac\ket{00} + ad\ket{01}+bc\ket{10}+bd\ket{11})$


## Density Operators

Let there be the following system
$\begin{matrix} \ket- & \ket i & \ket0 \\ \frac23 & \frac 16 & \frac 16 \end{matrix}$

This is a mixed ensemble
The fractions must all add up to 1

$P = P_1\ket\psi_1\bra\psi_1 + P_2\ket\psi_2\bra\psi_2+...+P_n\ket\psi_n\bra\psi_n$

For the system...
$P = \frac 23\ket-\bra- + \frac 16\ket i\bra i+\frac 16\ket0\bra0$

There are some properties...
1. Hermitian
2. Tr(p) = 1
3. P is positive semi definite, all eigenvalues are non-negitive

Thm P represents a pure ensemble iff $p^2 = p \text{ iff Tr}(p^2)=1$

Wiring Diagram
![[Wiring Diagram.png]]

![[WiringExample.png]]


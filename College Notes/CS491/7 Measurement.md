# Measurement Level 1
$\ket \psi = \alpha\ket0 + \beta\ket1$
Measure with respect to a basis $\ket0,\ket1$
$P_0=\left|\alpha\right|^2$ Probability $\ket0$ measured with respect to $\ket0,\ket1$
$P_1=\left|\beta\right|^2$ ""                $\ket1$

---
# Measurement Level 2  

**Measuring in an Arbitrary Orthonormal Basis**

---

## **State and Basis**:  
- Qubit state:  
  $\ket{\psi} = \alpha\ket{0} + \beta\ket{1}$  
- Instead of the standard basis $\{\ket{0}, \ket{1}\}$, you measure in **any orthonormal basis** $\{\ket{a}, \ket{b}\}$.  
  - Example bases:  
    - **Hadamard basis**: $\{\ket{+}, \ket{-}\}$ where  
      $\ket{+} = \frac{\ket{0} + \ket{1}}{\sqrt{2}}, \quad \ket{-} = \frac{\ket{0} - \ket{1}}{\sqrt{2}}$  
    - Any rotated basis (e.g., $\{\ket{\uparrow}, \ket{\rightarrow}\}$ for spin systems).  

---

## **Probabilities**:  
- The probability of measuring the qubit in state $\ket{a}$ or $\ket{b}$ is calculated by **projecting $\ket{\psi}$ onto the new basis**:  
  $P_a = |\langle a | \psi \rangle|^2, \quad P_b = |\langle b | \psi \rangle|^2$  
- **Example (Hadamard basis)**:  
  - Compute overlap with $\ket{+}$:  
    $\langle+|\psi\rangle = \frac{\alpha + \beta}{\sqrt{2}} \implies P_+ = \left|\frac{\alpha + \beta}{\sqrt{2}}\right|^2$  
  - Compute overlap with $\ket{-}$:  
    $\langle-|\psi\rangle = \frac{\alpha - \beta}{\sqrt{2}} \implies P_- = \left|\frac{\alpha - \beta}{\sqrt{2}}\right|^2$

---

## **Key Notes**:  
1. **Equivalent to rotating the state**:  
   - Measuring in $\{\ket{a}, \ket{b}\}$ is the same as:  
     1. Applying a **unitary transformation** $U$ to "rotate" the basis $\{\ket{a}, \ket{b}\}$ into $\{\ket{0}, \ket{1}\}$.  
     2. Measuring in the standard basis $\{\ket{0}, \ket{1}\}$.  
   - Example: To measure in the Hadamard basis, apply the $H$ gate (Hadamard gate) to the qubit *before* measuring in $\{\ket{0}, \ket{1}\}$.  

2. **Outcome**:  
   - After measurement, the qubit collapses to **either $\ket{a}$ or $\ket{b}$**, depending on the result.  

3. **Why use this?**  
   - Different bases reveal different properties of the qubit (e.g., diagonal vs. vertical polarization).  
   - Critical for protocols like **quantum teleportation** and **Bell state measurements**.  

---

## **Summary**:  
- **Level 1**: Measure in $\{\ket{0}, \ket{1}\}$ → probabilities depend on $|\alpha|^2$ and $|\beta|^2$.  
- **Level 2**: Measure in **any basis** $\{\ket{a}, \ket{b}\}$ → probabilities depend on projections $|\langle a|\psi\rangle|^2$ and $|\langle b|\psi\rangle|^2$.  
- Always involves an orthonormal basis (required for valid quantum measurements). 

**Spectral Decomposition Theorem:**
$\Omega=\lambda_1P_1+\lambda_2P_2+\lambda_3P_3$
$P_2\cdot P_1=P_1\cdot P_2=0$     $P_1\perp P_2$
$P_1=\bra\psi P_1 \ket\psi$
$P_2 = \bra\psi P_2 \ket\psi$


$\{eval, evec\} = Eigensystems[X]$

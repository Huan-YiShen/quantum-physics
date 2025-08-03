# Introuduction

## Information processing
- classical vs. quantum
- qubit (review)
  - computational basis state
  - superposition, bloch sphere
  - tensor product, entanglement
- Gates & Circuits
  - computational complexity
    - classical complexity classes: factorial, exponential, polynomial, linear-logarithmic, logarithmic, constant
    - quantum complexity classes: QMA, QMA-complete, BQP
  - Quantum Gates
    - universal gate set
    - specific example: Harnamard, CNOT, TOFFLE
    - measurements
  - Quantum Circuits
- error correction 
  - noise and coherence (T1, T2, fidelity) 



## The Qubit
Qubit is the fundamental unit of computing in quantum information processing. Analgous to classical bits, it has 2 states.

$$ \ket0 = 
\begin{bmatrix}
1 \\
0 
\end{bmatrix}
\text{ and }
\ket1 = 
\begin{bmatrix}
0 \\
1 
\end{bmatrix}
$$

Note: Different from classical bits we need to use a 2 dimensional array to represent a qubit. This is necessary to model qubits' superposition and entanglement behaviour. 

## Quantum Gates
universal gate set:
- in general, the formation of universal gate set contain
  - two distict single-qubit gates (so you can do arbitrary operations on the bloch sphere - superposition)
  - one two-qubit gate (enable entaglement) 


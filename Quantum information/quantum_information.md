# Introuduction
The study of Quantum information processing, at least its basic theory, does not require a deep understanding of quantum physics. There is a nice layer of abstraction between "The physics of building a device that exhabit quantum properties irl" vs. "what is quantum information processing and how can we use it". This layer of abstraction is the language of quantum mechanics, such as density operator and Dric notations. The underlying physics can be abstracted and the behaviour of this "quantum language" can be thought of as mathemtical axioms. In summary, the mathematical language of quantum mechanics will be the **interface** between quantum physics and quantum information.

It is here that our story begins, we will first study the langauge of quantum mechanics, most of this will be review from quantum physics. Then we will build up quantum information constructs (qubits, gates, circuits). Finally we will apply these constructs to build quantum information processing techniques (algorithms, communication protocols, etc...)

## Information processing topics
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
- Quantum Algorithms
- Quantum Communication
- Error Correction 
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


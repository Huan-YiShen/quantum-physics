# A two level system
Recall that any object in quantum mechanics is described by a *State Vector*

$$\ket{\Psi} = \sum_n c_n\ket{n} = \sum_n \ket{n}\braket{n|\Psi} $$

The above state vector exists in a discrete Hilbert space of dimension $n$ (hence the summation instead of an integral). 
The term $c_n = \braket{n|\Psi}$ represent the magnitude of the vector in $\ket n$ basis. To write down a two level system, simply set the number of dimensions $n=2$.

$$\ket{\Psi} = c_0\ket{0} + c_1\ket{1}$$

We can rewrite the above expression using vectors

$$\ket{\Psi} = c_0 
\begin{bmatrix}
1 \\
0 \end{bmatrix} + c_1
\begin{bmatrix}
0 \\
1 \end{bmatrix}$$

This system is interesting because many physical quantum system can be described as a 2 level system, such as electrons with spin 1/2. Furthermore it is useful in technology such as qubits.


# The Bloch Sphere
A nice way to visulize a two level system is using the Bloch Sphere. It uses two continuous parameters, similar to sperical coordinate system, to describe the probability of measuring state $\ket 0$ and state $\ket 1$.

$$\ket \Psi = cos \left( \frac{\theta}{2} \right) \ket 0 + e^{i\phi} sin \left( \frac{\theta}{2} \right) \ket 1$$


# Raising and Lowering Operators
One of the simplest operation we can perform on a two level system is to transition between the two states $\ket 0$ and $\ket 1$
- To raise from $\ket 0 \rightarrow \ket 1$, apply the tensor product $\ket 1 \bra 0$

$$(\ket 1 \bra 0) \ket 0 = \left( \begin{bmatrix}
0 \\
1 \end{bmatrix}
\otimes
\begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) \ket 0
= \begin{bmatrix}
0 & 0 \\
1 & 0 \end{bmatrix} \ket 0
= \begin{bmatrix} 
0 & 0 \\
1 & 0 \end{bmatrix}
\begin{bmatrix} 
1 \\
0
\end{bmatrix}
= \begin{bmatrix} 
0 \\
1
\end{bmatrix}
= \ket 1
$$

- To lower from $\ket 1 \rightarrow \ket 0$, apply the tensor product $\ket 0 \bra 1$

$$(\ket 0 \bra 1) \ket 1 = \left( \begin{bmatrix}
1 \\
0 \end{bmatrix}
\otimes
\begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) \ket 1
= \begin{bmatrix}
0 & 1 \\
0 & 0 \end{bmatrix} \ket 1
= \begin{bmatrix} 
0 & 1 \\
0 & 0 \end{bmatrix}
\begin{bmatrix} 
0 \\
1
\end{bmatrix}
= \begin{bmatrix} 
1 \\
0
\end{bmatrix}
= \ket 0
$$

The raising and lower operator is only sensible to one of the state in the 2 level system. Namely, the raising operator raises $\ket 0$ to $\ket 1$, but if it is applied to $\ket 1$, then it outputs a zero vector. 
This is obviously non-sensical since we cannot make $\ket 1$ disappear by applying an operator. But this does illustrate an important property in operators (to be discussed later).

# Pauli Matrices
three opeartors that describes the way a two level system can rotate on the surface of a Bloch Sphere

$$ \sigma_x = \begin{bmatrix}
0 & 1 \\
1 & 0 \end{bmatrix}
= \ket 0 \bra 1 + \ket 1 \bra 0$$

$$ \sigma_y = \begin{bmatrix}
0 & -i \\
i & 0 \end{bmatrix}
= i \left(-\ket 0 \bra 1 + \ket 1 \bra 0 \right)
= i \sigma_x \sigma_z$$

$$ \sigma_z = \begin{bmatrix}
1 & 0 \\
0 & -1 \end{bmatrix}
= i(\ket 0 \bra 0 - \ket 1 \bra 1)$$

To visulize the effect of each operators, use the right-hand-rule. Point the thumb along the positive axis and see the direction the fingers curve. For Pauli X opeartor ($\sigma_x$), point thumb towards the positive x-axis, and see how to finger rotates. 
It should be clear that a state vector pointing towards X ($\ket{\psi} = \frac{1}{\sqrt2} (\ket 0 + \ket 1$) would not have affect by Pauli X, but a $\ket 0 $ state would flip to $\ket 1$. 
In common 3D coordinate illustrations where z+ is up, y+ is right, and x+ is out of the page. 

Property of Pauli Matrix
* Hermitian
* Involutory
* Unitary
* Determinate = -1 for all
* Trace = 0 for all (they are all traces)
* Eigenvalue (all $\pm1$) & eigenvector
* Commutator relation (same as angular momentum) - they are closely related to the spin of 1/2 systems
* Anticommutator relation

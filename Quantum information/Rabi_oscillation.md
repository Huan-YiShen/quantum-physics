# Implement State Transition - Rabi Oscillation
Rabi oscillation is a way to **physically realize** state transitions of a two level system (i.e. how to convert $\ket 0$ to $\ket 1$ and vice versa). In particular, Rabi Oscillation specifies how to realize this in a semi-classical light-matter interacting system, this technique is the theory behind NMR and Trapped quantum computing controls.

We are going to start with a semi-classical description of the physical system. Namley an atom that acts as a two level system (quantum description), and a classical EM wave (monochromatic wave). At the end, we aim to construct an unitary opeartor that allows us to transition between the two levels (like an X gate).

## Semi-classical description of the the light-matter interaction
In this setup, we have an atom, modeled as a two level system

$$ \ket \Psi = c_0\ket 0 + c_1\ket 1$$

The time evolution of this system is described by the Shrondinger's Equation

$$ i\hbar\frac{d}{dt}\ket \Psi = H_0\Psi$$

where the Hamiltonian is of the following form

$$ H_0 = \begin{bmatrix}
E_1 & 0 \\
0 & E_2
\end{bmatrix} = E_1\ket 0\bra 0 + E_2\ket 1\bra 1$$

Notice that with this Hamiltonian, $\bra 0H\ket 1 = \bra 1H\ket 0 = 0$. This means that we have no way to transition between the two states, regardless how long we evolve the system.

Thus let us add an interacting Hamlitonian

$$ H_{tot} = H_0 + H_{int}$$

This interacting Hamiltonian comes form a laser light (monochromatic EM wave) shining on the atom. It is a time-dependent external radiation field 

$$H_{int} = -\mathbf{d \cdot E}(t)$$
* **d** is a dipole operator in 3 dmension
* **E**(t) is the monochromatic light in 3 dmension

Aside: Where did this formula for the interaction Hamiltonian came from?  This is a long story. Namely the dipolar approximation is used to remove the spatial dependency of the E field ([reference](https://mpl.mpg.de/fileadmin/user_upload/LectureNotes.pdf)). the dipoe opeartor describes the induced dipole the atom experience in the presence of an electric field, it is defined as $\mathbf d = \sum_i (charge)_i(distance)_i$

...
...
...

Solve the Shrodinger's equation with $H_{tot}$ to find its eigenvalue
...

Change to rotating frame of reference
...

Use Rotating wave approximation
...

Change the frame of reference again such that $H$ is time independent
...

Add time evolution operator to the system
...

Probability of transition from $\ket 0$ to $\ket 1$
...
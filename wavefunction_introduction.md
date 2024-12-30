# Intro to QM (wavefunction)
### The double slit experiment 
- This is a classic experiment that demostrate the `wave particle dulity` property of quantum particles. 
- This property cannot be explained with classical theory in physics. This experiment, among with others (such as the photoelectric effect), led physicists to develop a new theory aim to explain these new observations. This theory matured around the mid 20th centry, and was named quantum mechanics.

### The Wavefunction and Probability Distribution Function
The wavefunction $\Psi$
- Quantum physics describes the mechanics of *quantum systems* (quantum particles, their interactions, etc). 
- The state of a quantum system is described mathematically via the *wavefunction*.
- The wavefunction has position and time as inputs and a complex value as the ouput. It is commonly denoted by greek letter psi

$$\Psi(\vec x, t)$$

Physical interpretation of $\Psi$
- $\Psi$ itself does not represent anything physical, it is the solution of the Schrodinger's Equation.
- $\Psi$ contains information about the quantum system, and we can extract physical information from $\Psi$ by performing operations on it (such as an observation) - more on this later
- For example: one can extract the probability of the position of a quantum particle from $\Psi$ like the following

$$ P(\vec x) = |\Psi(\vec x, t)|^2$$

The amplitude square of the $\Psi$ satisfies the criteria of a probability distribution function (PDF). 
- like PDF, integrating it over all position will result in 1. it means that it is with 100% certainty that the particle will exist somewhere in space. The particle will not vanish, thus satisfies the conservation laws in nature.
- as to why $|\Psi(\vec x, t)|^2$ is a PDF is still an open question in physics. This line of question lead to the discussion of the different interpretations of quantum mechanics. Such as the *Copenhagen Interpretation* or the *Many World Interpretation*. But to understand those, we need to first understand the operators and the time evolution of wavefunctions.



### The Schrodinger's Equation
A differential equation that describes how the $\Psi$ evolves with time

$$i\hbar \frac{\partial \Psi(\vec x, t)}{\partial t} = \hat H \Psi(\vec x, t)$$

Where 
* $\hat H$ is the Hamlitonian of the system: $\hat H = -\frac{\hbar^2}{2m} \nabla^2 + V(\vec x, t) =$ kinetic energy + potential energy.
* $V(\vec x, t)$ is the potential energy of the system, it describes the environment the quantum system exists in
* $\Psi$ is the solution of this differetial equation

The discovery of this equation is quite funny:
- the wave equation:
- the diffusion eqation:
You combine them to make the Shrodinger's Equation

### Operator and Expectations of a measurement


### The uncertainty Relation between Position & Momentum


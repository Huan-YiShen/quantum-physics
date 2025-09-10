# topics
topic from J.J. Sakuri's text

### 1.2 Kets, Bras, and operators
- Ket space
  - Hilbert Space (everything is complex!)
  - discrete dimension and continuous spectra
  - state vector (ket as a representation of physical state)
  - linear combination (addition + scalar multiplication)
  - null ket
  - global phase (only "direction" in vector space is of significant)
  - observable = operator
  - eigenstate (eigenkets) and eignevalues
  - linear combination of basis

$$\ket a = \sum_b c_b \ket b$$

- Bra space and inner product
  - dual correspondence of ket space (also a space)
  - convert bra to ket (don't forget to take the complex conjugate)
  - inner product
    - $\braket{b|a} = \braket{a|b}^*$
    - $\braket{a|a} \ge 0$ (positive definite metric)
  - orthogonal 
    - two kets are orthogonal iff $\braket{a|b} = 0$
  - normalization of ket
    - ket is normalized iff $\braket{a|a} = 1$
    - $\sqrt{\braket{a|a}}$ = norm of $\ket a$

- Operators
  - equvalence in operators
  - null operator
  - "Addition of operators" is commutative and associative (1 exception)
  - dual of operator --> Hermitian adjoint --> **Hermitian**
- Multiplication
  - non-commutative && associative
  - $(XY)^\dagger = X^\dagger Y^\dagger$
  - **outer product** <-- $\ket a \bra b$
    - if $X\ket a$, then its dual is $\bra a X^\dagger$
- The associative Axiom of multiplication
  - $A\ket z = (\ket x \bra y) \ket z = \ket x \braket{y|z} = c\ket x$
  - if $X = \ket a \bra b$, then $X^\dagger = \ket b \bra a$
  - $\bra b X \ket a = \bra a X^\dagger \ket b ^*$

### 1.3 Base Kets and Matrix Prepresentations
- 1.3.1 Eigenkets of an observable
- 1.3.2 Eigenkets as Base Kets
- 1.3.3 Matrix representations
- 1.3.4 Spin 1/2 System
### 1.4 Measurements, Observables, and the Unvertainty Relation
- 1.4.1 Measurements
- 1.4.2 Spin 1/2 System
- 1.4.3 Compatible Observables
- 1.4.4 Incompatible Observables
- 1.4.5 The uncertainty relation
### 1.5 Change of basis
- 1.5.1 Transformation operator
- 1.5.2 Transformation matrix
- 1.5.3 Diagonalization
- 1.5.4 Unitary Equivalent Observables
### Position, Momentum, and translation
- 1.6.1 Continuous Spectra
- 1.6.2 Position Eigenkets and Position Measurements
- 1.6.3 Translation
- 1.6.4 Momentum as a Generator of Translation

# measurement and compatible observables

# The uncertain relation

# Translation and Generator (1.6.3)
  - define infinitesimal translation $T(dx) \ket x = \ket {x + dx}$
  - Define it in 3D
    - $T(dx) \int d^3 x (\ket{x} \braket{x|a}) = \int d^3 x (\ket{x+dx} \braket{x|a}) = \int d^3 x (\ket{x} \braket{x-dx|a})$
- alternative approach to translation: change of coordinate s.t. the origin is shifted in the opposite direction (-dx).

Now to construct this opeartor, we define some desired properties
  1. Output ket is normalized to unity
    - $\braket{a|a} = \bra a T^\dagger (dx) T(dx) \ket a$
    - iff T is unitary $T^\dagger (dx) T(dx) = I$
  2. Transitive?
    - $T(dx')T(dx) = T(dx' + dx)$
  3. Opposite-direction translation is the inverse
    - $T(-dx) = T^{-1}(dx)$
  4. Identity
    - $\lim_{dx\to 0}T(dx) = 1$
  5. Difference between $T(dx)$ and the identity operator be of first order in $dx$
    - Taylor expansion $T(dx) = dx + O(dx^2)$

Now to satisfy the above desired condition, define $T$ as the follow
$$T(dx) = 1-iKdx$$
- K need to be Hermitian, so with $i$, T can be unitary
- 1 and the $dx$ is to indicate that it is a infinitesimal change from the identity - property 5 is satified
- rest of the proeprty can be satified algebrically given property 5

$$[x, T(dx)] = dx \\
[x_i, K_j] = i\delta_{ij}$$
given above operators are 3D

# Probabilistic interpretation of QM
$\braket{a|b} \ge 0$ (positive definite metric), for all normalized kets $\braket{a|a} = 1$. Physically this means that ket exists somewhere with 100% probability. This is to conserve the conservation laws. 

Mathematically this means your Hilbert Space is large enough to describe all possible outcome of your quantum state. Your state must exist somewhere inside your Hilbert space. If it is less than 1, that means there is the porbability of your quantum state, exist outside of your Hilbert space.
